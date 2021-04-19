# codereviewgkcs
Code review examples for YouTube live with Gkcs.
```
//Reviewer must always be comfortable 
//You code must be self explanantory

public void constantsExample(){
	final String VALUE_9="9";//Bad practice 
	final String DOT_PNG=".png";//Bad practice

	final String LIMIT="9"//Good prcatice 
	final String EXTENSION=".png"//Good practice
	//Your code variable names must be self explanatory   
}

//constructs available to the user like ternary operators etc.
//can sometimes be unreadable as the user needs to create a mental map
//****Instead of writing clever code write simple code *****//

public void setDrivers(){
	User user=new User;
	List<User> drivers=new LinkedList<User>();
	List<User> nonDrivers=new LinkedList<User>();
	(user!=null) && (user.getAge()>=18)?drivers.add(user.getFirstName())
	:nonDrivers.add(user.getFirstName());
	//^^Completely correct code but not so readable 


	//better much more readble 
	if (user.isAllowedtoDrive()){
		drivers.add(user.getFirstName());
	}   
	else {
		nonDrivers.add(user.getFirstName());
	}
}
//Some tricks for performance 
//Example:---->
public void func(){
	int largest=getLargest();
	for (int i=0;i<getLargest();i++){
		if (curr>getLargest())
			curr=getLargest();
	}

	//getLargest is a very expensive function so call it only when absolutely 
	//necessary


}
// Tricks for performance:
//1. Use singletons and resource pools where you can 
//2. IO calls are expensive avoid them as much as possible 


//In java If you have a string that needs to altered multiple times 
//Try using StringBuilder/StringBuffer instead of String 
//To try and stop memory leakage 
//ORM object relations mapping

```

















