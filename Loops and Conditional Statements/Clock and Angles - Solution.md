# # Clock and Angles Solution

    def findclockangle(hour,minutes):
    	m = (360/60)*minutes
    	h = (360/12)*hour+ ((minutes/60)*(360/12))
    	c = abs(h-m)
    	
    	if c > 180:
    	  c = 360-c
    	  
    	return int(c)
    	
    for _ in range(int(input())):
      a , b = map(int,input().split())
      print(findclockangle(a,b))
