# TrainingReportLaTex
Template for Engineering Training Report according to University of Moratuwa Sri Lanka
This Template based on Industrial Training Book given by Faculty of Engineering University of Moratuwa

! Important: If you are not familiar with LaTex I recommend use classical MS word.

I used some comments on some places that you should change it and also some texts should be changed on your own.
Given report's example has been used "Times New Roman" font but they have mentioned in the document it seems like SF.

I tried this make as close as possible to given recommended style but you can change it your own :-).


\documentclass[12pt,a4paper]{report}
\usepackage{graphicx}
%margin 2.54cm = 1"
\usepackage[a4paper,hmargin={1in,1in},vmargin={1in,1in}]{geometry}
%line spacing 1.5
\linespread{1.5}
%paragraph spacing 3
\setlength{\parskip}{3pt}

%abbreviation
\newcommand{\abbrlabel}[1]{\makebox[3cm][l]{\textbf{#1}\ \dotfill}}
\newenvironment{abbreviations}{\begin{list}{}{\renewcommand{\makelabel}{\abbrlabel}}}{\end{list}}

\usepackage{floatrow}
\floatsetup[table]{capposition=top}
%\floatsetup[figure]{capposition=top}

%figures settings images should be added to images folder
\usepackage{float}
\graphicspath{{images/}}

\usepackage{enumitem}

%this can be used for applying codes for the documet 
% begin{listings} //Your Code// end{listings}
\usepackage{listings}
\usepackage{color}

\usepackage{titlesec}
\titleformat{\chapter}[display]   
{\normalfont\huge\bfseries}{\chaptertitlename\ \thechapter}{20pt}{\Huge}   
\titlespacing*{\chapter}{0pt}{-20pt}{20pt}

\definecolor{dkgreen}{rgb}{0,0.6,0}
\definecolor{gray}{rgb}{0.5,0.5,0.5}
\definecolor{mauve}{rgb}{0.58,0,0.82}
%Asiri Amal Karunanayaka

\lstset{frame=tb,
  language=Java,
  aboveskip=3mm,
  belowskip=3mm,
  showstringspaces=false,
  columns=flexible,
  basicstyle={\small\ttfamily},
  numbers=none,
  numberstyle=\tiny\color{gray},
  keywordstyle=\color{blue},
  commentstyle=\color{dkgreen},
  stringstyle=\color{mauve},
  breaklines=true,
  breakatwhitespace=true,
  tabsize=3
}

\begin{document}

\begin{titlepage}
\begin{center}
{\LARGE\textbf{{UNIVERSITY OF   MORATUWA}}\\[1cm]}
{{\LARGE Faculty of Engineering}}\\[2.25cm]
\includegraphics[width=2in, height=2in]{UOM.png}\\[2.25cm]
{{\LARGE Registered Module No: 3990 or 3992 or 3993}}\\[.35cm]
{\Large\textbf{{INDUSTRIAL TRAINING REPORT}}\\[.5cm]}
{\Large\textbf{{Your Company}}\\[1cm]}
{{\LARGE From 02/07/2018 to 07/12/2018}}\\[1.5cm]
{{\LARGE Date of Submission : 07/02/2019}}\\[1.5cm]
{{\LARGE Karunanayaka K.M.A.A.}}\\[.35cm]
{{\LARGE 150297K Department of Computer Science and Engineering}}\\[.35cm]
\end{center}
\end{titlepage}

\section*{Preface}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\newpage

\section*{Acknowledgment}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\tableofcontents

\listoffigures


\bigbreak
\begingroup
\let\clearpage\relax
\listoftables
\endgroup

%5-8 pages with SWOT analysis
\chapter{About Company}
\section{Company Overview}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum. 
\section{About your company 1}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\section{About your company 2}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{itemize}
\item[] Class I railroad systems
\end{itemize}

\section{Products and businesses}

$Lorem^{TM}$ Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\subsection*{Customers}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum. \cite{railroadClasses}.


\begin{itemize}
\item[] Class I  - Over $\$$200 million annual revenue.
\item[] Class II - Between $\$$100 to $\$$20 million annual revenue.
\item[] Class III - Less than $\$$20 million annual revenue.
\end{itemize}

\subsection*{Products}
\begin{enumerate}
\item product1 \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\item Product2
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\end{enumerate}


\begin{table}[!ht]
   \centering   \begin{tabular}{| c || c |}\hline \label{tbl:Product Explaining Sessions} 
		$Product$ & Conducted By \\ \hline
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$Product$ & Ms. ABC and Mr. XYZ\\
		$TMS$ & Mr. Mohommed Sabith\\ \hline
	\end{tabular}
   \caption{Product description sessions}
   \label{tab:ProductDescription}
\end{table}

\section{Organization Structure}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.


\subsection*{Rates$^{TM}$}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\begin{figure}[H]
\includegraphics[scale=.7]{Structure.png}
  \caption{Rates Organization Structure}
  \label{fig:Structure}
\end{figure}

\begin{itemize}
\item Concur \\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\item Rates
\begin{enumerate}
\item For Shippers\\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\item For Railroads\\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\end{enumerate}


\end{itemize}

\section{SWOT Analysis}
\subsection{Strengths}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\subsection{Weaknesses}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\subsection{Opportunities}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\subsection{Threats}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

%30-40 pages
\chapter{Training Experiences}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{table}[!ht]
   \centering   \begin{tabular}{| c || c |}\hline \label{tbl:Technical Training Sessions} 
		Technology & Conducted By \\ \hline
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\
		Session & Mr. ABC\\ \hline
	\end{tabular}
   \caption{Technical Training Sessions}
   \label{tab:TechnicalTraining}
\end{table}


\section{Scrum Practice}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\includegraphics[scale=.5]{Rally2.png}
  \caption{Rally Software}
  \label{fig:Rally2}
\end{figure}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\begin{figure}[H]
\includegraphics[scale=.5]{Rally1.png}
  \caption{Rally}
  \label{fig:Rally1}
\end{figure}

\begin{figure}[H]
\includegraphics[scale=.8]{Scrum.png}
  \caption{Scrum practice in Rates}
  \label{fig:Scrum}
\end{figure}




\section{Java Collection Framework}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{itemize}
	\item[$\ast$] Interfaces - List, Queue, Set, Deque, SortedSet
    \item[$\ast$] Classes - ArrayList, LinkedList, Vector, Stack, TreeSet, HashSet, LinkedHashSet
    
\end{itemize}

\begin{figure}[H]
\includegraphics[scale=.5]{JavaCollection.png}
  \caption{Java Collection Hierarchy}
  \label{fig:javaCollection}
\end{figure}
  
\begin{itemize}
	\item [List-]
	
	List has extended by three classes, ArrayList, LinkedList and Vector\\
	\begin{lstlisting}
	List<Object> myList = new ArrayList<object>();
	List<Object> myList = new linkedList<object>();
   \end{lstlisting}
	 Those both ArrayList and LinkedList have same method types,\\
	 \begin{lstlisting}
	 myList.add(obj1);
	 mylist.remove(obj1);
	 \end{lstlisting}
	 

But,\\ Linked lists good for numerous insertions and deletions.\\
Array lists better to use as store and accessing elements.
	
	
%	\item[Queue-]
%	\item[Set-]
\end{itemize}

\section{Java Generics}

In English "Generics" means, characteristic for group or set but it is not specific. Before java 5.0 there is no way to generalize object types the programmer always should have to manually set the object types. For example if we had made a method for \texttt{Strings} it can't be used for \texttt{Integers} unless integers can be implemented as a strings sometimes. But after J2SE 5.0\cite{bradbury2006mutation} they were designed extended type of objects can be allocated.

Since the java developer team has already used \{\} for coding and \texttt{"[]"} for lists newly introduces generics was represented by \texttt{"<>"}.

Three specific situations have been handled by generics;

\begin{itemize}
\item Compiler time type checker \\
Generics allows to identify type errors in compilation time and it is much more easier than identifying in runtime. 

\begin{lstlisting}
	List<Integer> myList = new LinkedList<>();
	myList.add(10);
	myList.add(3.14) //This will a generate compile time error
\end{lstlisting}

\item Redundant of type casting
Before generics we must use type casting for each and every time when it is called, 

\begin{lstlisting}
	List myList = new LinkedList();
	list.add("Generics");
	String out = (String) myList.get(0);}
\end{lstlisting}

But in Generics,
\begin{lstlisting}
	List<String> myList = new LinkedList<>();
	list.add("Generics");
	String out = myList.get(0);
\end{lstlisting}

\item Using none generic algorithms\\

We can do calculations on various types with have some similarities, this will provide type safety as well.
\end{itemize}
\subsection*{Usages of Generics}
\begin{enumerate}[label=(\roman*)]
\item Generic Classes\\
\begin{lstlisting}
//Java Generic class
	            public class MyClass<A> {
                private A a;
                public A getA() {
                    return a;
                }
                public void setA(A a) {
                    this.a = a;
                }
                public static void main(String[] args) {
                    MyClass<String>  a = new MyClass<>();

                    a.setA("Type"); //This "Type" must be String, 
                                    // Otherwise compile error will be occurred!
                    a.getA();
                }
            }

\end{lstlisting}

\begin{lstlisting}
//Generic class with Map
                import java.util.HashMap;
                import java.util.Map;
                
                public class GernericMap {
                    public static void main(String[] args) {
                
                        Map<Integer, Integer> integerMap
                                = new HashMap<Integer, Integer>();
                
                        integerMap.put(1, 10);
                        integerMap.put(2, 11);
                
                        Map<Integer, String> mixMap = new HashMap<>();
                
                        mixMap.put(23, "Hello");
                        mixMap.put(32, "World");
                    }
                }

\end{lstlisting}

\item Generic Methods\\

\begin{lstlisting}
//Java Generic Method
                public class MyClass<T> {
                    public static <T> boolean equals(MyClass<T> t1, MyClass<T> t2){
                        return t1==t2;
                    }
                }
\end{lstlisting}


\item Generic Interfaces\\

\begin{lstlisting}
//Java Generic Interface
                public interface MyInterface<T> {
                    public int isEqual(T o);
                }
\end{lstlisting}


\end{enumerate}


\section{Struts 2}

Struts 2 is mainly focused on MVC architecture it stands for Model, View and Controller.Struts 2 has been improved than Struts 1 like $Wild Cards$. 

\begin{itemize}
\item Model\\
Model Contains our business logic that means it has the actions to do.
\item View\\
This is the output of the view to the user. (In our company we use Smart GWT for this)
\item Controller\\
This contains the action class that interact user Model and View (Controller)
\item struts.xml
This file is the mapper for action and view.
\begin{lstlisting}
//struta.xml file\
        <?xml version="1.0" encoding="UTF-8" ?>
        <!DOCTYPE struts PUBLIC
                "-//Apache Software Foundation//DTD Struts Configuration 2.0//EN"
                "http://struts.apache.org/dtds/struts-2.0.dtd">
        <struts>
        <constant name="struts.devMode" value="true" />
        <package name="default" namespace="/" extends="struts-default">
        <action name="add.action"
        class="MyClass" method="addUser" >
        <result name="success">pages/customer.jsp</result>
        </action>
        </action>
        </package>
        </struts>
\end{lstlisting}
\end{itemize}

\section{Spring}
Spring can be represented as a framework of frameworks because it has the ability to support Struts, Hibernates and many other frameworks but Spring is lightweight framework. 

Here we are using the Spring framework to make the code loose coupling, It means this gives us to ability of dependency injection. 

\subsection*{Dependency Injection}
\begin{enumerate}
\item Constructor Based Dependency injection\\
In my experience in Company code base widely used this method, in here injection is attained by when the Constructor is invoked. The bean is created by \texttt{constructor-arg} in beans.xml file.
\begin{lstlisting}
//Example bean.xml
<?xml version = "1.0" encoding = "UTF-8"?>
<beans xmlns = "http://www.springframework.org/schema/beans"
        xmlns:xsi = "http://www.w3.org/2001/XMLSchema-instance"
        xsi:schemaLocation = "http://www.springframework.org/schema/beans
        http://www.springframework.org/schema/beans/spring-beans-3.0.xsd">
<bean id = "patronMaster" class = "com.PatronManager.PatronMaster">
<constructor-arg ref = "patronMasterImpl"/>
</bean>
</beans>
\end{lstlisting}

\item Setter Based Dependency injection\\
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum..xml file. In here beans.xml's \texttt{constructor-arg} has been replaced by \texttt{property name}.

\begin{lstlisting}
//beans.xml for setter based DI
<?xml version = "1.0" encoding = "UTF-8"?>
<beans xmlns = "http://www.springframework.org/schema/beans"
   xmlns:xsi = "http://www.w3.org/2001/XMLSchema-instance"
   xsi:schemaLocation = "http://www.springframework.org/schema/beans
   http://www.springframework.org/schema/beans/spring-beans-3.0.xsd">
   <!-- Definition for textEditor bean -->
   <bean id = "textEditor" class = "com.example.TextEditor">
      <property name = "spellChecker" ref = "spellChecker"/>
   </bean>
   <!-- Definition for spellChecker bean -->
   <bean id = "spellChecker" class = "com.example.SpellChecker"></bean>
</beans>
\end{lstlisting}
\end{enumerate}
\newpage
\section{Hibernate}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\centering
\includegraphics[scale=1]{Hibernate.png}
  \caption{Java Object Relational Mapping}
  \label{fig:ORM}
\end{figure}
\begin{lstlisting}
<?xml version = "1.0" encoding = "utf-8"?>
<!DOCTYPE hibernate-mapping PUBLIC 
"-//Hibernate/Hibernate Mapping DTD//EN"
"http://www.hibernate.org/dtd/hibernate-mapping-3.0.dtd"> 

<hibernate-mapping>
   <class name = "Employee" table = "EMPLOYEE">
      <meta attribute = "class-description">
         This class contains the employee detail. 
      </meta>
      <id name = "id" type = "int" column = "id">
         <generator class="native"/>
      </id>
      <property name = "firstName" column = "first_name" type = "string"/>
      <property name = "lastName" column = "last_name" type = "string"/>
      <property name = "salary" column = "salary" type = "int"/>
   </class>
</hibernate-mapping>
\end{lstlisting}

\section{Rates's Smart GWT 12 Upgrading}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\centering
\includegraphics[scale=.5]{RatesGWT4.png}
  \caption{Rates App Before GWT 12 Upgrade}
  \label{fig:RatesGWT4}
\end{figure}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\begin{figure}[H]
\centering
\includegraphics[scale=.4]{RatesGWT12.png}
  \caption{Rates App after GWT 12 Upgrade}
  \label{fig:RatesGWT12}
\end{figure}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\centering
\includegraphics[scale=.35]{NewUI.png}
  \caption{One page of the proposed user interface}
  \label{fig:NewUI}
\end{figure}

\subsection{Debugging via debugger mode}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
 
\begin{lstlisting}
\\Example css code for changes
			.normal, .normalFocused, .normalDisabled {
			    color: #282828;
			    font-family: RobotoLight;
			    font-size: 12px;
			}
\end{lstlisting}


\begin{figure}[H]
\centering
\includegraphics[scale=.4]{Debugging.png}
  \caption{Debugging in Google Chrome}
  \label{fig:Debugging}
\end{figure}

\subsection*{Smart GWT Showcase}
When developers need to check what are the exciting UI components Smart GWT is the most suitable place. Smart GWT showcase allows to get the latest versions of buttons, tables, interfaces and many more UI components.
\begin{figure}[H]
\centering
\includegraphics[scale=.35]{SmartGWTShowcase.png}
  \caption{Smart GWT Showcase}
  \label{fig:SmartGWTShowcase}
\end{figure}

\section{Creating a new Screen for Rates app}
I was given to crate a new Screen for hazardous materials (HAZMAT) called "IRF STCC Hasmat" in here IRF means Industry Reference File and STCC stands for Standard Transportation Commodity Code . Already "IRF STCC Master" screen has been created but it includes all the materials. Therefore project manager had decided to apply the hazardous materials to new screen.I had to manage client also the server side in this task.
\begin{itemize}
\item Client side
	\begin{itemize}
	\item Data Source - DS
	\item View Panel
	\end{itemize}

\item Server Side
	\begin{itemize}
	\item web
	\item service
	\item dao
	\item domain
	\end{itemize}
\end{itemize}

\subsection{Client Side}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\subsection{Server Side}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\begin{figure}[H]
\centering
\includegraphics[scale=.5]{Hazmat.png}
  \caption{IRF STCC Hazmat Screen}
  \label{fig:Hazmat}
\end{figure}

All commodities has a 7 digit response code and Hazmat response code can be easily identified with 49******* pattern. In Detail section all the valuable information has been listed to readability.

\subsection*{Good Programming practices in your Company}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\section{Creating Auto suggestion API}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\includegraphics[scale=.8]{PrefixSearch.png}
  \caption{Prefix based auto suggestion}
  \label{fig:PrefixSearch}
\end{figure}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
\begin{enumerate}
\item Database \\
Already MongoDB has already been integrated some developing parts therefore I  choose MongoDB as the Data base.
\item Algorithm\\
In my researches, two algorithms were founded. 
\begin{enumerate}
\item Splay tree algorithm
\item Trie tree algorithm
\end{enumerate}
\end{enumerate}

\subsection*{MongoDB}

MongoDB is not a traditional Relational Database Management system. MongoDB has no tables but collections these collections have documents with key value pairs this value can be any object. 

\begin{lstlisting}
//insering document for collection named "patronModel"
db.PatronModel.insert(            <------ Collection
        {  name = "ABC",
            age = "23",
           adderss = "los angelis"
}
)
\end{lstlisting}

To accomplish my task I wanted to convert these queries to java then I have chosen \texttt{Mongo Java driver 3.6}\cite{mongojavadriver} to type queries in java. 

\subsection*{Trie tree algorithm}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{itemize}
\item Trie tree uses small space comparing with others
\item Ideally each and every search has O(N) time complexity, here N stands for maximum string length.
\end{itemize}

Every Trie node has two main components, a map where the key is character and value is trie node and the second one is boolean end of word.

\begin{lstlisting}
			TrieNode{
			 Map<character, TrieNode> child;
			 boolean endOfWord;
			}
\end{lstlisting}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\begin{figure}[H]
\center
\includegraphics[scale=1]{TrieTree.png}
  \caption{Illustration of Trie tree}
  \label{fig:TrieTree}
\end{figure}

Here I have inserted \texttt{COMPUTER, COMMUNICATION, CONNECTION, INDUSTRY} and \texttt{INTELLIGENCE}. 

If I search \texttt{CO} this Trie tree will return texttt{COMPUTER, COMMUNICATION, CONNECTION} and node's attribute boolean endOfWorld will be true which has the character "O". 

I have created a database on MongoDB named with "SearchData" to accomplisg this task. My first task was add this for Patrons. Shipper, Consignee or Payer of Freight can be represented as a Patron. There is an existing method to fetch data from the Oracle database. For patrons these methods were spotted in PatronMasterManager class. This class had two methods to get data to the screen called singleFetchTask and groupFetchTask, then I wanted to add my method called favoriteFetchTask. 

I combined MongoDb and java with Mongo Java Driver to update the data and fetch data. For testing proposes I used user inputs and outputs. This was my initial testing it included for fields userName, userRole, field and userInput. This userInput duplicates the actual input from a text field. When a user enter a text in as userInput my algorithm find the all ancestors with the given prefix.

It takes me about two months to complete this task because most of the things done by my own. When completing this task I faced big problems with to matching the requirements I always with SSEs to keep in touch with my code. When I started to integrate the API, sometimes I faced some compatible problems as well. I did some changes hence it was completed. Finally I was assigned to integrate to some other places this API.

\newpage
\section{Events}

As a company Company has a welfare society, Toast masters club and other usual functions. Most of them are very entertained to me and I enjoyed very well. These kind of events are very helpful to build the connections with the employees as well.

\subsection*{The Toast Masters Club}

In Company TMC is very active club. Every two weeks on there is a TMC meeting in the lobby. All interns should participate that meeting. Most of the times interns actively participated to the meeting, and also the did some  roles too like time keeper, grammar checker and the contestants. One I participated a TMC club's contest as the official photographer.

\subsection*{Blood Donation Campaign}
A blood donation campaign held by the Welfare Society in October 11$^{th}$ 2018. This is a annual campaign. Most of the employees participated to donate the blood specially the interns too. 


\subsection*{Dinner out with Country manager}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\subsection*{Year end annual party}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.


%min 2pages
\chapter{Conclusion}
\section{Summery}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum. industry, my company was a product based company 
\section{Ability of providing training in Company}
Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

\section{Suggestions}

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.


\newpage
\section*{Abbreviations}
\begin{abbreviations}
\item[US] United States
\item[MIT] Massachusetts Institute of Technology
\item[CSXT] CSX-Transpotation ( A US railroad company)
\item[MRI] Magnetic Resonance Image
\item[CT] Computed Tomography 
\item[CEO] Chief Executive Officer
\item[GWT] Google Web Toolkit
\item[J2SE] Java 2 Standard Edition
\item[MVC] Model View Controller
\item[EDI] Electroonic Data Interchange
\item[POJO] Plain Old Java Object
\item[UI] User Interface
\item[HR] Human Resource
\item[NAITA] National Apprentice and Industrial Training Authority
\item[EDI] Electronic Data Interchange
\item[API] Application Programming Interface
\item[SQL] Structured Query Language
\item[IRF] Industry Reference File
\item[STCC] Standard Transportation Commodity Code 
\item[DS] Data Source
\item[DAO] Data Access Object
\item[CSS] Cascading Style Sheet
\item[TMC] Toast Masters Club
\end{abbreviations}

%here I have used references format as IEEE 
\renewcommand{\bibname}{References}
\bibliographystyle{IEEEtran}
\bibliography{IEEEabrv,References}








\end{document}
