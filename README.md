# codsoft2
tasks[]
def addTask() :
task = input("Please enter a task :") 
tasks. append(task) 
print("Task '{task}' added to the list ") 
def listTasks() :
if not tasks:
print(" There are no tasks currently ") 
else:
print(" Current tasks:") 
for index , task in enumerate(tasks) :
print("Task #{index} , {task}") 
def deleteTask() :
listTasks() 
try:
taskToDelete= int(input("Enter the # to delete:")) 
if taskToDelete >=0 and taskToDelete< len(tasks) :
tasks. pop(taskToDelete) 
print("Task {taskToDelete} has been removed") 
else:
print("Task #{taskToDelete} was not found ") 
except:
print(" Invalid input") 
if__name__=="__main__":
# create a loop to run the app 
print("Welcome to the to do list app:") 
while True:
print("\n") 
print("Please select one of the following options ") 
print(" 1.Add a new task") 
print("2.Delete a task") 
print("3. List tasks") 
print("4. Quit") 
ch= input("Enter your choice:") 
if (ch =="1") 
addTask() 
elif(ch=="2") :
deleteTask() 
elif(ch=="3") :
listTasks() 
elif(ch=="4") :
break:
print("Invalid input. Please try again") 
