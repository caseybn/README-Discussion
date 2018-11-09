# README-Discussion

## PURPOSE
    To demonstrate the importance of a good README, discuss the contents, review examples, and learn a few formatting tricks.

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
# 1. Project Description

# 2. Table of contents- especially important for longer README files 

# 3. Getting Started 
- Prerequisites: installation
- Challenges and solutions
- Resources

# 4. Usage/ Implementation
  - Helpful to include flow chart of code development
   
# 5. Example Code
```
# plot Budyko curve
x=seq(0,2,by=.00033)
n<-n

#aet_c=(ap*pet.ss)/((ap^n+pet.ss^n)^(1/n))

# plot Budyko curve
x=seq(0,2,by=.000333)
x<-x[1:6007]

y1<- x/((1+x^n)^(1/n)) #ecuation of Evaporative Index from Choudhury 1999. 
#y2<-x/((1+x^1.8)^(1/1.8))
bc<-data.frame(matrix(NaN,6007,1))#(dry,ei,aq,ap,apet,aet,AET.1,apet-aet)
a<-ggplot(data=bc)+aes(dry1,ei1)+theme_classic()+scale_x_continuous(expand = c(0,0),limits = c(0,2))+
  ggtitle("Budyko Curve at Hubbard Brook's WS3: Annual averages for water years 1959-2014")+
  scale_y_continuous(expand = c(0, 0),limits=c(0,1.1))+scale_shape_discrete(solid=F)+
  annotate("text", x = 0.6, y = 0.1, label = "PET/P<1 energy limited catchments")+
  annotate("text",x=1.4,y=0.1,label="PET/P>1 water limited catchments")+
  geom_point(aes(x=dry1,y=ei1),size=1,show.legend = FALSE)+
  geom_text(x=1.6,y=0.9,aes(label="n = 1.8 Forest Average (Choudhury, 1999)"), size=3.5)+
  geom_text(x=1.7,y=0.75,aes(label="n = 1.74 Calibrated n"), size=3.5)
b<-labs(x="Dryness Index (PET/P)",y="Evaporative Index (ET/P)",size=2)
c<-geom_segment(aes(x = 0, y = 0, xend = 1, yend = 1))
d<-geom_segment(aes(x=1,y=1,xend=2,yend=1))
e<-geom_segment(aes(x=1,y=0,xend=1,yend=1),linetype=2)
f<-geom_text(x=0.5,y=0.6,aes(label="Energy Limit",angle=60, size=1.5),show.legend = FALSE) #Water limit label
g<-geom_text(x=1.5,y=1.05,aes(label="Water Limit",size=1.5),show.legend = FALSE) #Energy Limit label
h<-geom_line(aes(x=x,y=y1))
i<-geom_line(aes(x=x,y=y2))
budyko<-a+b+c+d+e+f+g+h#+i
budyko
```

# 6. Example Output

![alt text](https://github.com/caseybn/README-Discussion/blob/master/Picture1.png)
![alt text](https://github.com/caseybn/README-Discussion/blob/master/Picture2.png)

# 7. Contributing (if necessary as part of a larger project)

# 8. Credits/ Acknowledgments 

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

