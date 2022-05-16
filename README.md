# R-2-2022.5.16
#问题1
#3-1 整数、浮点数、复数
#3-2 levels()
#3-3 as.numeric("6.283185")
#3-4 fix() View() edit()
#3-5 rm(list=is())
#问题2
#3-1类
class(Inf)
class(NA)
class(NaN)
class("")
#类型
typeof(Inf)
typeof(NA)
typeof(NaN)
typeof("")
#模式
mode(Inf)
mode(NA)
mode(NaN)
mode("")
#存储模式
storage.mode(Inf)
storage.mode(NA)
storage.mode(NaN)
storage.mode("")
#3-2
an<-sample(c("dog","cat","dolphin","hamster","glodfish"),100,replace = TRUE)
an[1:5]
table(an)

#3-3
bej<-c(apple<-1,avocado<-2,banana<-3,bennet<-4)
ls(pattern="a")
#问题3
#4-1
#a<-c(0,0.25,0.5,0.75,1,1.25)
#4-2
#方法1：赋值的时候直接命名
#efhu<-c(aeiu=3,efh=4,vul=5)
#方法2：利用names()函数
#names(efiq)[数字]<-value
#4-3
#正（负）整数索引；逻辑向量索引；名称索引；零值索引
#4-4
d1<-c("a1","a2","a3")
d2<-c("b1","b2","b3","b4")
d3<-c("c1","c2","c3","c4","c5","c6")
z<-array(1:72,c(3,4,6),list(d1,d2,d3))
z
length(z)
 #72
#4-5
#A$*%$t(A)
#问题4
#1
xl1<-seq(11,50,by=3)
xl1-c(2,3)
#2
xl2<-seq(1.1,4,by=20)
xl2*c(4,5,8,9)
#3
xl3<-c(1,2,4,6)
xl4<-c(8,0,-1,-4)
xl3+xl4
xl3-xl4
xl3*xl4
xl3/xl4
#问题5
#4-1
n<-(1:50)
triii<-c(n*(n+1)/2)
triii
names(triii)<-letters[1:15]
triii[c("a","e","i","o","u")]
#4-2
diaggg<-c(11,10,9,8,7,6,5,4,3,2,1,0,1,2,3,4,5,6,7,8,9,10,11)
diag(diaggg)
#问题6
#5-1
listtt<-list(alpha = 1, list(beta = 2, gamma = 3, delta = 4), eta = NULL)
listtt
print(length(listtt))
#5-2
(arguments_of_sd<-formals(sd))
$x
$na.rm
class(arguments_of_sd)
pairlist()
list()
#5-3
iqwef<-c(1,3,2)
iqwef[2]

wghh<-matrix(c(1,18,9,5,47,9),nrow=2,ncol=3)
wghh
wghh[2,1]

uhjj<-data.frame(v1=1:5,v2=6:10,v3=11:15)
uhjj
uhjj[uhjj$v1>2,]
#5-4
#列名必须是唯一且有效的变量名称。此功能可通过给 data.frame传入check.names = FALSE关闭
#5-5
d111=data.frame(c(1:3),c(3,2,1))
d222=data.frame(c(4:6),c(6,5,4))
d333=merge(d111,d222);
d333
#问题7
#5-1
m1<-matrix(0:99,nrow = 10,byrow = TRUE)
m1
list=apply(m1,MARGIN = 1,
  fuction(m1)
  {
    m1[round(sqrt(m1))^2==m1]
  }
)
list


#5-2
iris

dsvhb<-data.frame(iris[ ,1 ],iris[ ,2 ],iris[ ,3 ],iris[ ,4 ],row.names=NULL)
dsvhb
mean(iris[ ,1 ])
mean(iris[ ,2 ])
mean(iris[ ,3 ])
mean(iris[ ,4 ])
#5-3
attach(beaver1)
beaver1$id<-1
beaver1
attach(beaver2)
beaver2$id<-2
beaver2
beaaa=rbind(beaver1,beaver2);
subset(beaaa,activ==1)
