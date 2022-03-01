# CS205 C/C++ Program Design (S22) Assignment Grading Policy

<center>Feb. 23, 2022</center>

This is a C/C++ assignment rules, we will deduct scores according to this rule, but we will not strictly follow it all the time. In some cases, we may decide to detract more or less points based on the perceived gravity of the mistakes.[^1]

In C/C++ assignments, You are required to write **code and reports** and submit them to blackboard . We provide the standard of how we judge your assignments. There are several rules you need to follow.



## 1  Standard

| <span style="white-space:nowrap;">&emsp;&emsp;&emsp;&emsp;Standard&emsp;&emsp;&emsp;&emsp;</span> | <span style="white-space:nowrap;">&emsp;&emsp;&emsp;&emsp;Score&emsp;&emsp;&emsp;&emsp;</span> |
| :----------------------------------------------------------: | :----------------------------------------------------------: |
|                          Lab report                          |                              20                              |
|                      Output correctness                      |                              50                              |
|                        Error handling                        |                              20                              |
|                          Code style                          |                              10                              |

### 1.1   Notice

1. We strongly recommend you to **submit your assignments before deadline**. We will **deduct 20 scores each day** if you submit assignment after deadline. If you did not submit your assignment three days after deadline. You will get 0 for your assignment.
2. Please submit `.pdf` ﬁle for your report. If you do not submit the report or submit other types ﬁle such as `.doc` , `.docx` ,we will **deduct 10 scores**.
3. Please submit all your source code. If you do not submit all your source code *as specified in each assignment*, that makes your TAs could not run your program properly, you will be **deducted up to 80 scores**.
4. <span style="color:red">**No plagiarism.**</span> If we ﬁnd that you have plagiarized other's code or take the code from some websites strightly, you will get 0 scores for the assignment ; if we ﬁnd that you have plagiarized more than once, you will get 0 scores for the course. By the way, because we can't identify who copied whose code, if we ﬁnd that two students' code is similar, both of them will be punished.
5. The scores marked for each task in the document are raw scores. Your final score is
$$
\min(\Sigma_{task\text{ }}score * 0.7 + score_{report} + score_{code\text{ }style}, 100)
$$
6. You may notice that in some assignments, $\Sigma_{task\text{ }}score > 100$, which means:  [i] you may skip several tasks (but leaving a blank function body);  [ii] you may take the excess of 100 pts as a bonus and use it to offset other possible deductions.



## 2  Rules for score deduction

### 2.1   Compile and Run

1. Please specify your develop environment *especially when you are using some platform-dependent APIs* (e.g. `windows.h`). TA will try his best to run your code. If you do not specify the develop environment you are using, `-1` for each error.

   > 1. Please include this in both your **report** and the **bb comment**.
   > 1. For Windows users, if you are **not** using WSL, you may using `MSVC` / `mingw`;  for WSL / Linus users, you may using `gcc` / `g++`;  for macOS users, you may using `Apple clang` by default. If you are not sure about this, you may contact SAs.
   > 2. We will use `C++20` or `C17` standard to run your code. If you use a newer standard, like `C++23`, please also specify that.

2. If your code doesn't compile, we will deduct `10` scores.
3. If your code doesn't run , we will deduct `5` scores.

### 2.2   Output correctness <span style="color:red">[TODO]</span>

1. We will have multiple test cases. For each task, the score you get is 
1. 

### 2.3   Error handling <span style="color:red">[FIXME]</span>

1. Please make sure your code will not crash if the input is incorrect. Your code should give some notice when the input is incorrect (if not specified in the documentation, output some text in `stderr` that explains the cause of the error). Pay attention to input range and type.
1. If any **memory leak** is found, your score of the `Error handling` part will be deducted based on the perceived gravity of the mistakes.
1. If there are scoring rules for some tasks in the assignment document, the document will prevail.



### 2.4   Code style

Please pay more attention to your code style. After all this is not ACM-ICPC contest. You have enough time to write code with both correct result and good code style. You will get deduction if your code style is terrible. You can read [Google C++ Style Guide](https://google.github.io/styleguide/cppguide.html), [NASA C Style Guide](https://ntrs.nasa.gov/api/citations/19950022400/downloads/19950022400.pdf) or some other guide for code style. Here are some bad examples:

```cpp
void gao();  // bad function name
int a, aa, aaa;  // bad variable name
void main(){
  
}  // bad main function

							vector<int> vec;
			vec.push_back(1);
				for(auto& element:vec)
    std::cout<<element<<std::endl;
// bad spacing
```



[^1]: This rule will take eﬀect from the date of publication.
