# CS 210 LAB 07: Choc-O-Holic, Inc. (Singleton Pattern)

Everyone knows that all modern chocolate factories have computer-controlled chocolate boilers. The job of the boiler is to take in chocolate and milk, bring them to a boil, and then pass them on to the next phase of making chocolate bars.

Check out the controller class for Choc-O-Holic, Inc.’s industrial strength Chocolate Boiler. You’ll notice they’ve tried to be very careful to ensure that bad things don’t happen, like draining 500 gallons of unboiled mixture, or filling the boiler when it’s already full, or boiling an empty boiler!

## Step 1: Test one controller

Review the `ChocolateBoiler.java` class, noting the validations that have been put in place for each method.

Then, review the `Main.java` class, which has a test scenario already staged for us.

Go ahead and run the program.

## Step 2: Test two controllers

Uncomment the second test in Main.java, where we have created a second ChocolateBoiler object.  Now there are TWO CONTROLLERS connected to the same physical boiler.

If we run the program now, and each controller tries to fill the boiler, does it still stop the second fill attempt, or does it allow it?

## Step 3: Apply Singleton Pattern

Update the `ChocolateBoiler.java` class, implementing the Singleton pattern such that even if we try to create multiple ChocolateBoiler objects, we only have ONE connection to the physical boiler.

Update `Main.java` as needed and run the tests again.
