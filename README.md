# week-3-b-median
me <- function(m){
  x <- length(m)
  if(x%%2==0){
    mid <- m[x%/%2]+m[(x%/%2)+1]
    return(mid/2)
  }else{
    mid <- m[(x%/%2)+1]
    return(mid)
  }
}
med=scan()
m <- sort(med)
median <- me(m)
print(median)
median(med)



OUTPUT:
> me <- function(m){
+   x <- length(m)
+   if(x%%2==0){
+     mid <- m[x%/%2]+m[(x%/%2)+1]
+     return(mid/2)
+   }else{
+     mid <- m[(x%/%2)+1]
+     return(mid)
+   }
+ }
> med=scan()
1: 5
2: 6
3: 9
4: 2
5: 4
6: 3
7: 
Read 6 items
> m <- sort(med)
> median <- me(m)
> print(median)
[1] 4.5
> median(med)
[1] 4.5
> 
