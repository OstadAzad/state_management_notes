# state_management_notes

📌 1. Short Notes – Key Points:
State মানে হলো একটি ডেটা বা অবস্থা যা সময়ের সাথে পরিবর্তিত হতে পারে।

State Management হলো state গুলিকে কোথায়, কিভাবে রাখা হবে এবং কিভাবে পরিবর্তন করা হবে তা নিয়ন্ত্রণ করা।

মূলত ৩ ধরনের স্টেট থাকে: Local, Global, Server State।

ভালো state management মানে কম Bug, পরিষ্কার কোড, সহজ ডিবাগিং।

📘 2. Concept Explanation
🔸 State কী?
State হলো এমন তথ্য যা আপনার অ্যাপের UI-কে পরিবর্তিত করে। উদাহরণ: লাইক বাটনে ক্লিক করলে সংখ্যা বাড়ে, এটিই state পরিবর্তন।

স্টেট কি?
স্টেট হলো একটি জাভাস্ক্রিপ্ট অবজেক্ট যা কম্পোনেন্টের ডাটা স্টোর করে এবং UI-কে রিফ্লেক্ট করে।

🔸 State কোথায় রাখা হয়?
Local State: ছোট ছোট component-এর ভিতরে (useState React এ)

Global State: অনেক জায়গা থেকে একসাথে access করার জন্য (Redux, Context API)

Server State: API থেকে আনা ডেটা যা সার্ভারে থাকে (যেমন React Query, SWR)

🔸 State Management কেন দরকার?
আপনার অ্যাপ যত বড় হবে, তত বেশি স্টেট থাকবে। সব জায়গা থেকে state একসাথে কন্ট্রোল করতে হলে state management দরকার হয়।

স্টেট হলো ডাইনামিক ডাটা যা UI কে আপডেট করে।

স্টেট ম্যানেজমেন্ট অ্যাপ্লিকেশনকে স্কেলযোগ্য করে।

💡 3.Examples – Explained:
// React useState example
const [count, setCount] = useState(0);
ব্যাখ্যা: count নামের একটি state রাখা হয়েছে, যা 0 থেকে শুরু হয়। setCount দিয়ে তা পরিবর্তন হয়।

✅ Project 1: Counter App (Local State)
Features: Increase / Decrease button
Solution:
const [count, setCount] = useState(0);
<button onClick={() => setCount(count + 1)}>+</button>
<button onClick={() => setCount(count - 1)}>-</button>

✍️ 4. Exercise Tasks with Detailed Solutions:
🔹 Task 1: Form Input Value Save
Input Box + Show live input
const [name, setName] = useState('');
<input onChange={(e) => setName(e.target.value)} />
<p>Your name is: {name}</p>


Name : Azad
Contact : 01814-868644
email : azads5390@gmail.com
Don't waste paper. Save the tree.
