A01Q4
=====
int getlen(struct node *head)
{
struct node *temp=head;
int len=1;
while(temp)
{
temp=temp->next;
len++;
}
return len;
}
void getnode(struct node*head, int len, int n)
{
struct node*temp=head;
int count=0;
while(count!=len-n)
{
temp=temp->next;
count++;
}
printf("%d",temp->data);
}

