# Project1
the first week's homework
N=50;
head=0;
tail=0;
total=0;
run=0;
run1=0;
  for i=1:N
      total=total+1;
      a=rand();
      if a>=0.5
          head=head+1;
          run1=run1+1
      else
          tail=tail+1;
          if run1>run
              run=run1
              run1=0
          else
              run1=0
          end
      end
      
  end
  p=head/N
B=[head tail];
figure(1)
bar(B,0.2);
figure(2)
bar(B,0.3)
