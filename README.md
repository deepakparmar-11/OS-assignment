# OS-assignment

16.	A barrier is a tool for synchronizing the activity of a number of threads.When a thread reaches a barrier point, it cannot proceed until all otherthreads have reached this point as well. When the last thread reachesthe barrier point, all threads are released and can resume concurrentexecution.

Assume that the barrier is initialized to N—the number of threads thatmust wait at the barrier point: init(N);

Each thread then performs some work until it reaches the barrier point:

/* do some work for awhile */ barrier point();

/* do some work for awhile */

Using synchronization tools like locks, semaphores and monitors, construct a barrierthat implements the following API:

• intinit(int n)—Initializes the barrier to the specified size.

• int barrier point(void)—Identifies the barrier point. All threads are released from the barrier when the last thread reaches this point.
