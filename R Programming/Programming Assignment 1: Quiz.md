Quiz
Q1. What value is returned by the following call to pollutantmean()? You should round your output to 3 digits.
```{r}
pollutantmean("specdata", "sulfate", 1:10)
```
Q2. What value is returned by the following call to pollutantmean()? You should round your output to 3 digits.
```{r}
pollutantmean("specdata", "nitrate", 70:72)
```
Q3. What value is returned by the following call to pollutantmean()? You should round your output to 3 digits.
```{r}
pollutantmean("specdata", "sulfate", 34)
```
Q4. What value is returned by the following call to pollutantmean()? You should round your output to 3 digits.
```{r}
pollutantmean("specdata", "nitrate")
```
Q5. What value is printed at end of the following code?
```{r}
cc <- complete("specdata", c(6, 10, 20, 34, 100, 200, 310))
print(cc$nobs)
```
Q6. What value is printed at end of the following code?
```{r}
cc <- complete("specdata", 54)
print(cc$nobs)
```
Q7. What value is printed at end of the following code?
```{r}
set.seed(42)
cc <- complete("specdata", 332:1)
use <- sample(332, 10)
print(cc[use, "nobs"])
```
Q8. What value is printed at end of the following code?
```{r}
cr <- corr("specdata")                
cr <- sort(cr)                
set.seed(868)                
out <- round(cr[sample(length(cr), 5)], 4)
print(out)
```
Q9. What value is printed at end of the following code?
```{r}
cr <- corr("specdata", 129)                
cr <- sort(cr)                
n <- length(cr)                
set.seed(197)                
out <- c(n, round(cr[sample(n, 5)], 4))
print(out)
```
Q10. What value is printed at end of the following code?
```{r}
cr <- corr("specdata", 2000)                
n <- length(cr)                
cr <- corr("specdata", 1000)                
cr <- sort(cr)
print(c(n, round(cr, 4)))
```
