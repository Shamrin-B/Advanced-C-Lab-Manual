EXP NO:11 C PROGRAM TO DISPLAY STACK ELEMENTS USING AN ARRAY.

Aim:
To write a C program to display stack elements using an array.
Algorithm:
1.	Include Necessary Header Files
2.	Declare Global Variables
3.	Define the Display Function
4.	Main Function (or Other Relevant Code)
5.	Initialize the stack and top as needed.
6.	Perform stack operations (push, pop, etc.).
7.	Use the display function to visualize the stack's contents
 
Program:

```
char stack[50];
int top,i;
void display()
{
    for(i=top;i>=0;i--)
    {
        printf("%c ",stack[i]);
    }
    
}
```


Output:



<img width="410" height="198" alt="492404809-b32fa0ad-cc60-47db-af92-28a522b56fa8" src="https://github.com/user-attachments/assets/bb2b7ad5-37e2-4c00-8173-63023efea6fc" />

Result:
Thus, the program to display stack elements using an array is verified successfully.
 

EXP NO:12  PROGRAM TO PUSH THE GIVEN ELEMENT IN TO A STACK USING ARRAY.
Aim:
To create a C program to push the given element in to a stack using array.
Algorithm:
1.	Declare global variables for the stack size, top index, and the stack itself.
2.	Define the push function to add a floating-point number to the stack.
3.	Initialize the stack size, top index, and the stack itself.
4.	Call the push function as needed.
 
Program:

```
int size=3,top=-1;
float stack[100];
void push (float data)
{
    if(top==size-1)
    {
        printf("stack is full");
    }
    else
    {
        top++;
        stack[top]=data;
    }
}
```
Output:
<img width="411" height="198" alt="492404916-dec9b052-8703-4077-83c0-88942ac086bd" src="https://github.com/user-attachments/assets/06c4ff82-6ff5-477d-bbb9-d7d0fdfcb680" />





Result:
Thus, the program to push the given element in to a stack using array is verified successfully


 
EXP NO:13 C PROGRAM TO DISPLAY QUEUE ELEMENTS USING ARRAY.
Aim:
To write a C program to display queue elements using array

Algorithm:
1.	Declare global variables for the queue, rear, front, and iteration.
2.	Define the display function to print the elements of the queue.
3.	Initialize the queue, rear, and front as needed.
4.	Call the display function and perform other queue operations as needed.
 
Program:

```
int front,rear;
char queue[50];
void display()
{
    if(front==-1 || front>rear)
    {
        printf("No elements to display\n");
    }
    else
    {
    for(int i=front;i<=rear;i++)
    {
        printf("%c\n",queue[i]);
    }
    }
}
```

Output:

<img width="688" height="604" alt="492405027-88c1dd8c-1581-4812-b827-425155e7a261" src="https://github.com/user-attachments/assets/6906fb18-a857-4616-a752-fd3366f998a8" />



Result:
Thus, the program to display queue elements using array is verified successfully.


 
EXP NO:14 C PROGRAM TO INSERT ELEMENTS IN QUEUE USING ARRAY.
Aim:
To write a C program to insert elements in queue using array.

Algorithm:
1.	Declare global variables for the size, rear, front, and the queue itself.
2.	Define the enqueue function to add a float to the queue.
3.	Initialize the rear, front, and size of the queue as needed.
4.	Call the enqueue function as needed.

Program:
```
int size=10, rear=-1, front=-1;
float queue[50];
void enqueue(float data)
{
    if(rear<size)
    {
        if(front==-1)
        {
            front=0;
        }
        rear=rear+1;
        queue[rear]=data;
    }
}
```
Output:


<img width="768" height="448" alt="492405211-dd1d7b64-e660-4d61-aa55-5d2ea800305b" src="https://github.com/user-attachments/assets/353c6e20-9fd5-4d35-babe-a1865e01bf4d" />




Result:
Thus, the program to insert elements in queue using array is verified successfully.



 
EXP NO:15 C FUNCTION TO DELETE ELEMENTS IN QUEUE USING ARRAY



Aim:

To create a function in C that deletes an element from a queue implemented using an array.

Algorithm:

1.	Check if the Queue is Empty
o	If the front pointer is -1, it means the queue is empty, and there are no elements to delete. Print a message indicating that the queue is empty.
2.	Delete the Front Element
o	If the queue is not empty, the element at the front index is deleted.
o	Increment the front pointer by 1 to remove the element and point to the next element in the queue.
3.	Check if the Queue Becomes Empty After Deletion:
o	After deletion, check if the front pointer has passed the rear pointer (front > rear). If this is true, reset both front and rear to -1, indicating that the queue is now empty.
4.	End the Function.



Program:
```
float queue[50];
int front, rear;
void dequeue()
{
    if(front==-1||front>rear)
    {
        printf("\nNo elements to display");
    }
    else
    {
        front++;
    }
}
```


Output:

<img width="709" height="424" alt="492405395-8160399e-7510-4f81-8252-9ad2f982ae60" src="https://github.com/user-attachments/assets/9efc8eee-dd15-49bc-b080-a2627e81672f" />


Result:
Thus, the function that deletes an element from a queue implemented using an array is verified successfully.
