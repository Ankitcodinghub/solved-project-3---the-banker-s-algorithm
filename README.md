# solved-project-3---the-banker-s-algorithm
**TO GET THIS SOLUTION VISIT:** [SOLVED:Project 3 – The banker’s algorithm](https://www.ankitcodinghub.com/product/solvedproject-3-the-bankers-algorithm/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;1543&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SOLVED:Project 3 – The banker’s algorithm&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
PROJECT 3*********************************************

The source codes: Bank.java BankImpl.java TestHardness.java

can be compiled and run from the command line

(or)

can be copy pasted (or imported) into an IDE, under a new project

(or)

the NetBeans project (Project3) can be importedinto NetBeans directly.

NOTE: Make sure that infile.txt is containedwithin the same folder as your source codesto ensure that the file will be found atruntime.

*********************************************

Note: Please rename Bank.txt, BankImpl.txt, and TestHardness.txt to Bank.java, BankImpl.java and TestHardness.java. For this project, we will complete Project Banker’s algorithm as it is described Banker’s algorithm: The resource-allocation-graph algorithm is not applicable to a resource allocation system with multiple instances of each resource type.The deadlock avoidance algorithm that we describe next is applicable to such a system but is less efﬁcient than the resource-allocation graph scheme. This algorithm is commonly known as the banker’s algorithm. The name was chosen because the algorithm could be used in a banking system to ensure that the bank never allocated its available cash in such a way that it could no longer satisfy the needs of all its customers. When a new process enters the system, it must declare the maximum number of instances of each resource type that it may need. This number may not exceed the total number of resources in the system. When a user requests a set of resources, the system must determine whether the allocation of these resources will leave the system in a safe state. If it will, the resources are allocated; otherwise, the process must wait until some other process releases enough resources. Several data structures must be maintained to implement the banker’s algorithm. These data structures encode the state of the resource-allocation system. We need the following data structures, where n is the number of processes in the system and m is the number of resource types: • Available . A vector of length m indicates the number of available resources of each type. If Available [j] equals k, then k instances of resource type Rj are available. • Max. Ann × m matrix deﬁnes the maximum demand of each process. If Max[i][j] equals k, then process Pi may request at most k instances of resource type Rj. • Allocation.An n×m matrix deﬁnes the number of resources of each type currently allocated to each process. If Allocation [i] [j] equals k, then process Pi is currently allocated k instances of resource type Rj. Deadlocks • Need. Ann × m matrix indicates the remaining resource need of each process. If Need [i] [j] equals k,then process Pi may need k more instances of resource type Rj to complete its task. Note that Need [i] [j] equals Max[i] [j] −Allocation[i][j]. These data structures vary overtime in both size and value. To simplify the presentation of the banker’s algorithm, we next establish some notation. Let X and Y be vectors of length n. We say that X ≤ Y if and only if X[i] ≤ Y[i] for alli = 1, 2, …, n. For example, if X = (1,7,3,2) and Y = (0,3,2,1), then Y≤X. In addition, Y &lt; X if Y≤X and Y=X. We can treat each row in the matrices Allocation and Need as vectors and refer to them as Allocation and Need. The vector Allocation speciﬁes the resources currently allocated to process Pi; the vector Need speciﬁes the additional resources that process Pi may still request to complete its task. 1 Safety Algorithm We can now present the algorithm for ﬁnding out whether or not a system is in a safe state. This algorithm can be described as follows: 1. Let Work and Finish be vectors of length m and n, respectively. Initialize Work = Available and Finish[i]=false for i = 0, 1, …, n−1. 2. Find an index i such that both a. Finish[i] ==false b. Need ≤Work If no such i exists, go to step 4. 3. Work = Work + Allocation Finish[i]=true Go to step 2. 4. If Finish[i] ==true for all i, then the system is in a safe state. This algorithm may require an order of m×n2 operations to determine whether a state is safe. 2 Resource-Request Algorithm Next,we describe the algorithm for determining whether requests can be safely granted. Let Request be the request vector for process Pi. If Request [j] == k, then process Pi wants k instances of resource type Rj. When are quest for resources is made by process Pi, the following actions are taken: 1. If Request ≤ Need,go to step 2 . Otherwise,raise an error condition,since the process has exceed edits maximum claim. 2. If Request ≤ Available, go to step 3. Otherwise, Pi must wait, since the resources are not available. 3. Have the system pretend to have allocated the requested resources to process Pi by modifying the state as follows: Available= Available- Request; Allocation = Allocation + Request; Need = Need – Request; If the resulting resource-allocation state is safe, the transaction is completed,and process Pi is allocated its resources.However,if then ew state is unsafe, then Pi must wait for Request, and the old resource-allocation state is restored. 3.3 An Illustrative Example To illustrate the use of the banker’s algorithm, consider a system with ﬁve processes P0 through P4 and three resource types A,B,and C. Resource type A has ten instances, resource type B has ﬁve instances, and resource type C has seven instances.Suppose that,at time T0,the following snap shot of the system has been taken: Allocation Max Available A B C A B C A B C P0 0 1 0 7 5 3 3 3 2 P1 2 0 0 3 2 2 P2 3 0 2 9 0 2 P3 2 1 1 2 2 2 P4 0 0 2 4 3 3 The content of the matrix Need is deﬁned to be Max − Allocation and is as follows: Need ABC P0 743 P1 122 P2 600 P3 011 P4 431 We claim that the system is currently in a safe state. Indeed, the sequence &lt;P1, P3, P4, P2, P0 satisﬁes the safety criteria. Suppose now that process P1 requests one additional instance of resource type A and two instances of resource type C, so Request1 = (1,0,2). To decide whether this request can be immediately granted, we ﬁrst check that Request1 ≤ Available—that is, that (1,0,2) ≤ (3,3,2), which is true. We then pretend that this request has been fulﬁlled, and we arrive at the following new state: Allocation Need Available A B C A B C A B C P0 0 1 0 7 4 3 2 3 0 P1 3 0 2 0 2 0 P2 3 0 2 6 0 0 P3 2 1 1 0 1 1 P4 0 0 2 4 3 1 We must determine whether this new system state is safe. To do so, we execute our safety algorithm and ﬁnd that the sequence &lt;P1, P3, P4, P0, P2 satisﬁes the safety requirement. Hence, we can immediately grant the request of process P1. You should be able to see,however, that when the system is in this state,a request for(3,3,0)by P4 cannot be granted,since the resources are not available. Furthermore, a request for (0,2,0) by P0 cannot be granted, even though the resource sare available, since the resulting state is unsafe. We leave it as a programming exercise for students to implement the banker’s algorithm. 1.Read the project description thoroughly before you do anything else. Project description: The Bank The bank will employ the strategy outlined earlier, whereby it will consider requests from n customers for m resources. The bank will keep track of the resources using the following data structures: int numberOfCustomers; // the number of customers int numberOfResources; // the number of resources int[] available; // the available amount of each resource int[] [] maximum; // the maximum demand of each customer int [] [] allocation; // the amount currently allocated // to each customer int[ ] [] need; // the remaining needs of each customer The implementation of this interface will require adding a constructor that is passed the number of resources initially available. For example, suppose we have three resource types with 10, 5, and 7 resources initially available. In this case, we can create an implementation of the interface using the following technique: Bank the Bank = new BankImpl(10,5,7); The bank will grant a request if the request satisﬁes the safety algorithm outlined . If granting the request does not leave the system in a safe state, the request is denied. Testing Your Implementation You can use the ﬁle TestHarness.java, which is available on Wiley Plus, to test your implementation of the Bank interface. This program expects the implementation of the Bank interface to be named BankImpl and requires an input ﬁle containing the maximum demand of each resource type for each customer.For example,if there are ﬁve customers and three resource types,the input ﬁle might appear as follows: 7,5,3 3,2,2 9,0,2 2,2,2 4,3,3 This indicates that the maximum demand for customer0 is 7,5,3;for customer1, 3,2,2; and so forth. Since each line of the input ﬁle represents a separate public interface Bank {/** * Add a customer * customerNumber – the number of the customer * maximumDemand – the maximum demand for this customer */ public void addCustomer (int customerNum, int[] maximumDemand); /** * Output the value of available, maximum, * allocation, and need */ public void getState(); /** * Request resources * customerNumber – the customer requesting resources * request – the resources being requested */ public boolean request Resources(int customerNumber, int[] request); /** * Release resources * customerNumber – the customer releasing resources * release – the resources being released */ public void release Resources(int customer Number, int[] release); } customer, the addCustomer() method is to be invoked as each line is read in, initializing the value of maximum for each customer.(In the above example,the value of maximum [0] is initialized to 7,5,3 for customer 0;maximum[1][]is initialized to 3,2,2; and so forth.) Furthermore, TestHarness.java also requires the initial number of resources available in the bank. For example, if there are initially 10, 5, and 7 resources available, we invoke TestHarness.java as follows: java Test Harness infile.txt 10 5 7 where infile.txt refers to a ﬁle containing the maximum demand for each customer followed by the number of resources initially available. The available array will be initialized to the values passed on the command line. 2.Your job is to fill out the BankImpl.java file with hints given in the code. Please periodically test your functions as best as you can. 0. Once things start working, you can use the Test Harness program that is included. To run it, type Java TestHarness infile.txt 10 5 7 Or Create a new project configuration from run à set project configuration, and set arguments to be infile.txt 10 5 7. If you input * and press Enter, it will tell you the current state of your bank (as output by your getState() method). If you type RQ 0 2 2 2 then customer 0 will request two of each available resource. Likewise, RL 0 2 2 2 will make customer 0 release two of each resource. Here is an example of my output: run: * Available [10 5 7] Allocation [0 0 0] [0 0 0] [0 0 0] [0 0 0] [0 0 0] Max [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 3 3] Need [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 3 3] RQ 4 2 3 5 *2* *3* *5* Customer # 4 requesting 2 3 5 Available = 10 5 7 Approved * Available [8 2 2] Allocation [0 0 0] [0 0 0] [0 0 0] [0 0 0] [2 3 5] Max [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 3 3] Need [7 5 3] [3 2 2] [9 0 2] [2 2 2] [2 0 -2] RL 4 2 2 2 *2* *2* *2* Customer # 4 releasing 2 2 2 Available = 10 4 4 Allocated = [0 1 3 ]* Available [10 4 4] Allocation [0 0 0] [0 0 0] [0 0 0] [0 0 0] [0 1 3] Max [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 3 3] Need [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 2 0] RQ 0 1 3 2 *1* *3* *2* Customer # 0 requesting 1 3 2 Available = 10 4 4 Denied * Available [10 4 4] Allocation [0 0 0] [0 0 0] [0 0 0] [0 0 0] [0 1 3] Max [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 3 3] Need [7 5 3] [3 2 2] [9 0 2] [2 2 2] [4 4 6]
