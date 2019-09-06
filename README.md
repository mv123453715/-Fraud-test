# -Fraud-test
# 這是針對信用卡的詐欺檢測 
# 目標：可以利用被詐欺的歷史資料找到詐欺手法的規律  預防下一次相同的詐欺模式
# 欄位說明
time : 時間   
v1-v28: 脫敏數據 信用卡必要組成數據   
amout: 交易數量   
class:分類 0代表安全 1代表詐欺   


+ [資料來源] : (https://www.kaggle.com/mlg-ulb/creditcardfraud/home )


Sun Wu and Udi Manber 
Fast 
i-. i 
Errors 
The string-matching problem is a very common problem. 
We are searching for a string P = PtP2.. "Pro inside a large text 
file T = tlt2...t., both sequences of characters from a finite 
character set Z. The characters may be English characters in a 
text file, DNA base pairs, lines of source code, angles between 
edges in polygons, machines or machine parts in a production 
schedule, music notes and tempo in a musical score, and so 
forth. We want to find all occurrences of P in T; namely, we 
are searching for the set of starting positions F = {i[1 
--- i--- n - m + 1 such that titi+ l""ti+ m - 1 = P}" The two most 
famous algorithms for this problem are the Boyer-Moore 
algorithm [3] and the Knuth Morris Pratt algorithm [10]. 
There are many extensions to this problem; for example, we 
may be looking for a set of patterns, a pattern with "wild 
cards," or a regular expression. String-matching tools are 
included in every reasonable text editor, word processor, 
and many other applications. 
In some instances, however, the 
pattern and/or the text are not 
exact. For example, we may not 
remember the exact spelling of a 
name we are searching, the name 
may be misspelled in the text, the 
text may correspond to a sequence 
of numbers with a certain property 
and we do not have an exact pat-
tern, the text may be a sequence of 
DNA molecules and we are looking 
for approximate patterns. The 
approximate string-matching prob -" 
lem is to find all substrings in T that 
are close to P under some measure 
of closeness. The most common 
measure of closeness is known as 
the edit distance (also the 
Levenshtein measure [13]). A string 
P is said to be of distance k to a 
string Q if we can transform P to be 
equal to Q with a sequence of k in-
sertions of single characters in (ar-
bitrary places in) P, deletions of sin-
gle characters in P, or substitutions 
of characters. In some cases we may 
want to define closeness differently. 
For example, a policeman may be 
searching for a license plate 
ABC123 with the knowledge that 
the letters are correct, but there 
may be an error with the numbers. 
In this case, a string is of distance 1 
to ABC123 if only one error occurs 
and it is within the digits area. 
Maybe there are always three digits 
in a license plate, in which case only 
substitutions are allowed. Some-
times one wants to vary the cost of 
the different edit operations, say 
deletions cost 3, insertions 2, and 
substitutions 1. 
Many different approximate 
string-matching algorithms have 
been suggested ([4, 5, 6, 8, 11, 12, 
16, 19, 20] is a partial list). In this 
article we present a new algorithm 
which is very fast in practice, rea-
sonably simple to implement, and 
supports a large number of varia-
tions of the approximate string-
matching problem. The algorithm 
is based on a numeric scheme for 
exact string matching developed by 
COMMUNICATIONS OF THE ACM/October 1992/Vol.35, No.10 83
