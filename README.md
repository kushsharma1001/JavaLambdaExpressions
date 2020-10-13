# JavaLambdaExpressions
Lambdas in Java 8

https://youtu.be/MqsCdbMQjWc

interface #Predicate{ //Predicate is functional interface with one method only which takes 1 argument and returns a boolean.
boolean test(T);
}
Example Usecase: void printConditionally(List<Person> personList, Predicate<Person> predicate) {
                    for(Person p : presonList){
                      if(predicate.test(p)
                          System.out.println(p);
                    }
                  }

interface #Supplier{ //Supplier is functional interface with one method only which doesnt take arguments and returns a object of type T.
T get();
}

function{ //takes in type T and returns another type R.
 R apply(T);
}
