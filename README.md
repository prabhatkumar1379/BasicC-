# BasicC-
# ❓ Question 1: What are Data Types in C#?

---

## 📖 Definition
A **data type** in C# defines:
- What kind of data a variable can hold.
- How much memory it occupies.
- The range of values.
- The operations that can be performed.

---

## 🔹 Types of Data Types

### 1. Value Types
- Store the **actual data directly**.
- Stored in **Stack memory**.
- Each variable has its own copy (independent).
- Examples: `int`, `float`, `char`, `bool`, `struct`.

### 2. Reference Types
- Store a **reference (address)** to the actual data.
- Reference is in **Stack**, actual object in **Heap**.
- Multiple variables can point to the same object.
- Examples: `string`, `class`, `object`, `array`.

### 3. Pointer Types
- Store memory addresses (used in **unsafe context**).
- Rare in managed C# code.

---

## 📝 Example Code

```csharp
// Value Type Example
int number = 10;        // Value stored directly in Stack
bool isActive = true;   // Holds true directly in Stack

// Reference Type Example
string name = "Prabhat";     // Reference in Stack → actual string in Heap
int[] scores = {90, 80, 70}; // Array object is reference type → stored in Heap

// Struct Example (Value Type)
struct Point
{
    public int X;
    public int Y;
}
Point p1 = new Point();
p1.X = 5; 
p1.Y = 10;  // Struct fields stored directly in Stack
