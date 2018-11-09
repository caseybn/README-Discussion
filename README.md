# README-Discussion

## PURPOSE
To demonstrate the importance of a good README, discuss the contents, review examples, and 

## WHY READMEs ARE IMPORTANT
1. **Engages others in the project**
2. *Explains why the project is important*
3. Gives others the opportunity improve upon the work
4. **_Allows new users the ability to utilize your work for personal use_**

## WHAT MAKES A GOOD README
- Informative Project Title
- Descriptive summary of the overall project
- Efficiently informative, yet concise
- Common issue and solutions
- Example code and explanation 

## README Contents
1. Project Description

2. Table of contents- especially important for longer README files 

3. Getting Started 
- Prerequisites: installation
- Challenges and solutions
- Resources

4. Usage/ Implementation
  - Helpful to include flow chart of code development
   
5. Example Code
```
recoding_function <- function(jl_vector){

if(jl_vector[55] == 1){ #if ancestor is equal to 1...

(jl_vector[1:55][jl_vector[1:55] == 1] <- 444) #change all 1s to placeholder 444

(jl_vector[1:55][jl_vector[1:55] == 0] <- 1) #change all 0s to orginal ancestor (1)

(jl_vector[1:55][jl_vector[1:55]== 2] <- -1) #now change all 2s to -1

(jl_vector[1:55][jl_vector[1:55]== 444] <- 0) #now change all 444s to 0
} else if(jl_vector[55] == 2) { #if ancestor is equal to 2...

(jl_vector[1:55][jl_vector[1:55] == 2] <- 888) #change all 2s to placeholder 888

(jl_vector[1:55][jl_vector[1:55] == 0] <- 2) #change all 0s to original ancestor (2)

(jl_vector[1:55][jl_vector[1:55]== 2] <- -1) #now change all 2s to -1

(jl_vector[1:55][jl_vector[1:55]== 888] <- 0) #now change all 444s to 0
} else if(jl_vector[55] == 0){ #if ancestor line is 0...

(jl_vector[1:55][jl_vector[1:55]==2] <- -1) #change all 2s to -1
}

return(jl_vector)

}
```

6. Example Output 

7. Contributing (if necessary as part of a larger project)

8. Credits/ Acknowledgments 

## EXAMPLES
[Example of a bad README](https://github.com/sinwar/flaskr)

[Example of a good README](https://github.com/sindresorhus/pageres)

## IMAGES
- Images must be stored in your repo to include them in your README
![alt text](https://github.com/caseybn/README-Discussion/blob/master/G%26G.jpg)

## Helpful Links
[GitHub Writing and Formatting Help](https://help.github.com/articles/basic-writing-and-formatting-syntax/)

[Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)

https://medium.com/@meakaakka/a-beginners-guide-to-writing-a-kickass-readme-7ac01da88ab3

