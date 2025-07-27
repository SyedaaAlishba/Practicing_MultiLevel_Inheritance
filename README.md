<h1>Lets Learn MultiLevel Inheritance</h1>
<h3> What is Multilevel Inheritance?</h3>
<p>Multilevel inheritance means a class inherits from a class, which itself inherits from another class. Like a chain.</p>
<h3>🧩 What This Code Demonstrates:</h3>
<p>This Java program demonstrates multilevel inheritance, using the example of animals. It models the inheritance structure as:
Animal → Mammal → Dog / Cat
Each level of the hierarchy inherits behavior from the previous one and adds or overrides its own.
🔹 Animal is abstract – it provides shared structure (name, noise) and common behavior (eat()), but it forces subclasses to implement walk() and makeNoise() methods.
🔹 The constructor Animal(String name) sets the name of the animal.
🐾 2. Intermediate Class – Mammal
🔹 Mammal extends Animal.
🔹 It implements the abstract methods walk() and makeNoise() from Animal.
🔹 super(name) in Mammal calls the constructor of Animal to set the name.
🐶 3. Subclass – Dog
🔹 Dog extends Mammal, forming the third level in the inheritance chain.
🔹 The constructor chain is:
Dog(name) → Mammal(name) → Animal(name)
🔹 The makeNoise() method is overridden to say "Wof WOf".
🐱 4. Subclass – Cat
🔹 Cat is just like Dog, but overrides makeNoise() differently and renames this.name manually.
🚀 5. Program Runner – Run
- This class creates and runs both a `Dog` and a `Cat`.
- Calls their methods to demonstrate:
- Inherited behaviors (`walk`, `eat`)
- Overridden methods (`makeNoise`)
🏁 6. Main Class – Main
🔹 The entry point of the program. It simply creates an object of Run and runs it.
</p>
