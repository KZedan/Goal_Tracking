# My Problem Breakdown processes
1. Write user stories from the requirements
  * These should be user-centric, with a clear statement of value that this feature will give them
2. Extract the nouns and verbs from the first user story
3. Nouns are the objects, verbs are the messages or methods to send to the objects
4. Build a table of the ```objects```and```methods```

   For example...

   | **Object** | **Methods** |
   |------------|-------------|
   | controller |             |
   | passenger  |             |
   | plane      | flying?     |
   | airport    | land_plane  |
5. Map the ```methods``` to ```objects``` to see which messages can be sent to which objects
6. Draw out how they need to interact (and how the individual objects should encapsulate their concerns)
7. How would the user expect to use the program
  * Run through an example in a REPL, for example
  ```2.5.0 :001 > airport = Airport.new(10)
  => #<Airport:0x00007fd90a8cab00 @planes=[], @capacity=10>

  2.5.0 :002 > plane1 = Plane.new
  => #<Plane:0x00007fd90a8e2138>

  2.5.0 :003 > airport.land_plane(plane1)
  => [#<Plane:0x00007fd90a8e2138>]```
8. Write down a series of the simplest things to build up from (these could eventually become your tests)
Below example from roman numeral converter

return a single type (string)
converts 0 to “”
converts 1 to “I”
converts 2 to “II”
converts 5 to “V”
9. Each object can be a separate file
10. Further modelling can support a greater understanding of the problem, how the domain is structured, and how the parts of the eventual solution need to interact. This can include
  * Class models to represent the relationships between objects in your model
  * Sequence diagrams to model each delegation to a different object or system with your application. They highlight information about what each message returns and what objects will call them
