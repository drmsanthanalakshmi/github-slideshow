def tr_rec(i):
....if i>0:
.......result=i+tr_rec(i-1)
....else:
.......result=0
....return result
print(tr_rec(6))

steps:
when tr_rec(i) called
if i >0 then it goes to result=i + tr_rec(i-1)
unilt i =0 it will recursively called tr_rec(i)
then it will

example:
=tr_rec(6)
= 6 + tr_rec(5)
= 6 + (5 + tr_rec(4))
= 6 + (5 + (4 + tr_rec(3)))
= 6 + (5 + (4 + (3 + tr_rec(2))))
= 6 + (5 + (4 + (3 + (2 + tr_rec(1)))))
= 6 + (5 + (4 + (3 + (2 + (1 + tr_rec(0))))))
= 6 + (5 + (4 + (3 + (2 + (1 + 0)))))
= 6 + (5 + (4 + (3 + (2 + 1))))
= 6 + (5 + (4 + (3 + 3)))
= 6 + (5 + (4 + 6))
= 6 + (5 + 10)
= 6 + 15
= 21

return 21
