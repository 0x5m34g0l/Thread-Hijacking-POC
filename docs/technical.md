The technique involves:

1- Opening target process with appropriate privileges

2- Allocating executable memory for shellcode

3- Creating remote thread in suspended state

4- Saving original thread context

5- Redirecting instruction pointer to shellcode

6- Resuming thread execution

(Optional) Restoring original execution flow
