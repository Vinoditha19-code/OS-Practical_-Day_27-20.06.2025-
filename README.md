# OS-Practical_-Day_27-20.06.2025-
Question_01: 
Conclusion,
    The program creates two threads using the pthread library.
    Each thread prints a message indicating it is running.
    The main thread waits for both threads to finish using pthread_join.
    Ensures that the main program does not exit before the threads complete.
    Demonstrates basic thread creation, execution, and synchronization in C.
    
  ![Q1](https://github.com/user-attachments/assets/5aaba54a-65d4-4a66-8b0a-b74e1c4120e9)

Question_02:
Conclusion,
    The program creates 5 threads concurrently.
    Each thread prints its own unique thread ID.
    The main thread waits for all threads to finish using pthread_join.
    After all threads complete, a final completion message is printed.
    This demonstrates managing multiple threads and synchronizing their completion in C using pthreads.

![Q2](https://github.com/user-attachments/assets/a2f670c3-222a-4de3-9d93-d74122dd6923)


Question_03:
Conclusion,
    The program creates a single thread that counts from 1 to 10.
    The thread prints each number with a 1-second delay (sleep(1)) between prints.
    The main thread waits for the counting thread to finish using pthread_join.
    After the counting thread completes, the main thread prints a completion message.
    Demonstrates thread creation, timed execution, and synchronization with the main thread.

![Q3](https://github.com/user-attachments/assets/47d4dd3a-635f-43d9-afe8-ab17b62fc4ea)


Question_04:
Conclusion,
    Two threads are created: one increments a global counter 100 times, the other decrements it 100 times.
    A mutex (pthread_mutex_t lock) is used to ensure exclusive access to the counter, preventing race conditions.
    Each thread locks the mutex before modifying the counter and unlocks it afterward.
    Both threads print a message when they finish their operation.
    The main thread waits for both threads to complete using pthread_join.
    After both threads finish, the final value of the counter is printed (expected to be 0).
    The program demonstrates synchronization of shared data using mutexes in a multithreaded environment.

![Q4](https://github.com/user-attachments/assets/3a2bb2cf-07e2-4491-9fe2-5e766e34c823)


Question_05:
Conclusion,
    The program creates a thread that receives an integer argument.
    The thread function calculates the square of the given integer.
    The result is dynamically allocated and returned to the main thread using pthread_exit.
    The main thread retrieves the result via pthread_join and a pointer to the returned value.
    After printing the squared result, the main thread frees the allocated memory.
    Demonstrates passing arguments to threads and returning values safely using dynamic memory in pthreads.

  ![Q5](https://github.com/user-attachments/assets/94a6ad8e-02ed-4453-9501-5593c51a98bc)
