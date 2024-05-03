#include<stdio.h>
#include<stdlib.h>
struct node
{
      int data;
      struct node *left;
      struct node *right;
};
struct node* createNode(int d)
{
      struct node *temp=(struct node*)malloc(sizeof(struct node*));
      temp->left=NULL;
      temp->right=NULL;
      temp->data=d;
      return temp;
 }
 struct node* insert(struct node *root,int d)
 {
       if(root==NULL)
       {
            root=createNode(d);
       }
       else
       {
          if(d<root->data)
          {
              root->left=insert(root->left,d);
           }
           else if (d>root->data)
           {
                root->right=insert(root->right,d);
           }
           }
           return root;
  }
  void display(struct node *root)
  {
     if(root!=NULL)
     {
         display(root->left);
         printf(" %d",root->data);
         display(root->right);
      }
  }       
  int main()
  {
       int d;
       struct node *root=NULL;
       root=insert(root,50);
       root=insert(root,20);    
       display (root);                         
  }    
