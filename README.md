# INTERACTIVE-QUIZ-APPLICATION
COMPANY:CODTECH IT SOLUTIONS

NAME:RUPALI NAMDEV DHAMALE

INTERN ID:CT08ITV

DOMAIN:FRONT END DEVELOPMENT

DURATION:4 WEEKS

MENTOR:NEELA SANTOSH

 Description
 I Build the application using HTML, CSS, and JavaScript.
 for that purpose i used visual studio code editior to build quize application.
 
 1.User Registration: Users can register and create an account to track their progress.
2. Quiz Categories: Quizzes can be categorized by topic (e.g., history, science, sports).
3. Quiz Questions: Each quiz consists of a series of multiple-choice questions.
4. Interactive Interface: Users can interact with the quiz through a user-friendly interface.
5. Score Tracking: Users can view their scores and progress after completing a quiz.
6. Leaderboard: A leaderboard displays the top-scoring users.

A quiz application can serve various purposes and offer numerous benefits to users. It can be an engaging and interactive way to learn new concepts, subjects, or skills, helping students prepare for exams, assessments, or certifications. Additionally, quizzes can be used to assess a user's knowledge, understanding, or skills in a particular area, identifying strengths, weaknesses, and areas for improvement.


![Image](https://github.com/user-attachments/assets/8d59e2e5-dada-4930-bc97-af8f55088539)

![Image](https://github.com/user-attachments/assets/44740684-053c-49c1-96f0-61c1df90893d)









import java.util.*;

public class TokenRing {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Number Of Nodes You Want In The Ring : ");
        int n = sc.nextInt();

        System.out.println("Ring Formed Is As Below: ");
        for (int i = 0; i < n; i++) {
            System.out.print(i + " ");
        }

        System.out.println("0");

        int choice = 0;

        do {
            System.out.print("Enter Sender : ");
            int sender = sc.nextInt();

            System.out.print("Enter Receiver : ");
            int receiver = sc.nextInt();

            System.out.print("Enter Data To Send : ");
            int data = sc.nextInt();

            int token = 0;

            System.out.print("Token Passing : ");

            for (int i = token; i <= sender; i++) {
                System.out.print(" " + i + "->");
            }

            System.out.println(" " + sender);
            System.out.println("Sender: " + sender + " Sending Data: " + data);

            for (int i = sender; i != receiver; i = (i + 1) % n) {
                System.out.println("Data: " + data + " Forwarded By: " + i);
            }
        System.out.println("Receiver: " + receiver + " Received The Data: " + data);

       token = sender;

        System.out.print("Do You Want To Send Data Again? If YES Enter 1, If NO Enter 0");
        choice = sc.nextInt();
     }while(choice == 1);
    }
}
