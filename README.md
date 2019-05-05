# project-01-group-05
group-05-project-1-5 created by GitHub Classroom  

# Mean gene expression of all 27 samples  

nrow(expression)  
[1] 49070  

mean.exp = data.frame(mean_expression = 1:49070)  
rownames(mean.exp) = rownames(expression)  


for (i in 1:49070) {  
     s = 0  
     for (a in 1:27) {  
         s = s + expression[i, a]  
     }  
     mean.exp[i, 1] = (s / 27)  
 }  
rm(a)
rm(s)