# Time-calculation-through-classes-in-python
class Time():
    def __init__(self,hours,min):
        self.hours=hours
        self.min=min
    def addTime(self,ob1,ob2):
         ob.min=ob1.min+ob2.min
         ob.hours=ob1.hours+ob2.hours
         while(ob.min>=60):
                ob.min = ob.min - 60
                ob.hours=ob.hours+1
         return ob
    def displayTime(self,obj):
        print("Addition of time of two objects :", obj.hours, 'hours', obj.min, 'minutes')
    def DisplayMinute(self,hr,min):
        while(hr>0):
            hr=hr-1
            min=min+60
        print("Total minutes in time: ",min,"minutes")
ob=Time(0,0)
ob1=Time(2,50)
ob2=Time(1,10)
print("object 1 time: ",ob1.hours,'hours',ob1.min,'minutes')
print("object 2 time: ",ob2.hours,'hours',ob2.min,'minutes')
ob.displayTime(ob.addTime(ob1,ob2))
ob.DisplayMinute(1,2)
