Ahmad Khoshvaght 401422081

۱)بله این امکان وجود دارد. با تقسیم عدد به دو عدد با نصف تعداد ارقام و سپس استفاده از فرمول زیر میتوان تعداد ضرب هارا از n2 برای دو عدد n رقمی به nlog(n کاهش پیدا می‌کند.
A = 1234
B = 4321
C = A*B = 5332114

a0 = 34
a1 = 12

b0 = 21
b1 = 43

c0 = a0*b0
c1 = (a0+a1)*(b0+b1) - (c0+c2)
c2 = a1*b1
C = c2*10000 + c1*100 + c0
همانطور که میبینید به این روش با تکنیک بازگشنی میتوان از انجام ۱۶ ضرب اعداد ۱ رقمی در هم به ۹ ضرب (۳تا برای مرحله اول و ۲ تا ۳ ضرب دیگر برای ۲ زیر مرحله) رسید.




۲) کوچکترین زیر مسله برای این مسله ضرب دو عدد ۱ رقمی یا ضرب یک عدد ۲ رقمی در یک عدد ۱ رقمی (در حالتی که تعداد ارقام فرد باشد) می‌باشد.





۴) با توجه به اینکه در هر مرحله recursion تعداد ارقام نصف می‌شود پس یک log n داریم.
در هر مرحله با بهینه سازی میتوان گفت که به تعداد n/2 حدودا ضرب داریم.
در نتیجه پیچیدگی زمانی الگوریتم n log n می‌شود.