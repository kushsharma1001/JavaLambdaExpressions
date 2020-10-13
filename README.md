# JavaLambdaExpressions
Lambdas in Java 8

https://youtu.be/MqsCdbMQjWc

//Predicate is functional interface with one method only which tests 1 argument and returns a boolean.
interface #Predicate{ 
boolean test(T);
}
**Example Usecase: 
                  void printConditionally(List<Person> personList, Predicate<Person> predicate) {
                    for(Person p : presonList){
                      if(predicate.test(p)
                          System.out.println(p);
                    }
                  }
  
Use like: printConditionally(people, p-> p.getFirstName.equals("Rahul")); //Assume a person class with firstName and lastName instance variables.**

//Supplier is functional interface with one method only which doesnt take arguments and returns an object of type T.
interface #Supplier{ 
T get();
}

//takes in type T and returns another type R.
function{ 
 R apply(T);
}

//Consumer accepts one argument and returns nothing.
interface Consumer{
  accept();
  }

