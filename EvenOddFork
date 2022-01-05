#include<stdio.h>
#include<stdlib.h>
#include<sys/types.h>
#include<unistd.h>
#include<sys/wait.h>
int main(int argc, char *argv[])
{
    pid_t pid;
    pid = fork();
    if(pid < 0)
    {
        perror("Fork failed ");
    }
    if(pid == 0)
    {
        printf("\n Child process \n");
        printf("I am a child with process id %d\n" , (int) getpid());
        
         printf("Even numbers are : "); 
        for(int i=1;i<=10;i++)
        {
          
          if(i%2==0)
          {
              printf("%d , ",i);
          }
        }
       // exit(0);
    }
    printf(" \nI am parent process with id %d\n",(int) getpid());
     printf("odd numbers are : "); 
        for(int i=1;i<=10;i++)
        {
          
          if(i%2==1)
          {
              printf("%d , ",i);
          }
        }
    printf("\n Parent Ending ....\n");
    return 0;

}