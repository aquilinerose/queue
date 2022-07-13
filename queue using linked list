#include<stdio.h>
#include<stdlib.h>
void main()
{
	struct node
	{
		int data;
		struct node *next;
	};
	struct node *front=NULL,*rear=NULL,*del=NULL,*pos=NULL;
	int ch,a,i=0;
	while(1)
	{
		int ch;
		printf("enter your choice\n1.enqueue\n2.dequeue\n3.display\n4.exit\n");
		scanf("%d",&ch);
		switch(ch)
		{
			case 1:
			{
				printf("enter element");
				scanf("%d",&a);
				if(front==NULL)
				{
					front=(struct node*)malloc(sizeof(struct node));
					front->data=a;
					pos=front;
					rear=front;
				}
				else
				{
					rear->next=(struct node *)malloc(sizeof(struct node));
					rear->next->data=a;
					rear=rear->next;
				}
				i++;
				break;
			}
			case 2:
			{
				del=front;
				front=front->next;
				free(del);
				i--;
				break;
			}
			case 3:
			{
				pos =front;
				printf("the elements are\n");
				while(pos!=NULL)
				{
					printf("%d\n",pos->data);
					pos=pos->next;
				}
				break;
			}
			case 4:
			{
				printf("good bye");
				exit(0);
			}
		}
	}
}
		

