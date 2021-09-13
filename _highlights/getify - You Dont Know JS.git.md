# You Dont Know JS.git
by getify

45 unrecognized

---

* When we fake multitasking, such as trying to type something at the same time we’re talking to a friend or family member on the phone, what we’re actually most likely doing is acting as fast context switchers. In other words, we switch back and forth between two or more tasks in rapid succession, simultaneously progressing on each task in tiny, fast little chunks. We do it so fast that to the outside world it appears as if we’re doing these things in parallel.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1592-1595 | Aggiunto in data giovedì 17 maggio 2018 13:41:23</sup></p>

* If you have code that uses callbacks, especially but not exclusively with third-party utilities, and you’re not already applying some sort of mitigation logic for all these inversion of control trust issues, your code has bugs in it right now even though they may not have bitten you yet. Latent bugs are still bugs.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1774-1776 | Aggiunto in data sabato 19 maggio 2018 13:33:17</sup></p>

* If you have code that uses callbacks, especially but not exclusively with third-party utilities, and you’re not already applying some sort of mitigation logic for all these inversion of control trust issues, your code has bugs in it right now even though they may not have bitten you yet. Latent bugs are still bugs.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1774-1776 | Aggiunto in data sabato 19 maggio 2018 13:33:26</sup></p>

* For example, regarding more graceful error handling, some API designs provide for split callbacks (one for the success notification, one for the error notification):

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1778-1780 | Aggiunto in data sabato 19 maggio 2018 13:34:43</sup></p>

* But what if we could uninvert that inversion of control? What if instead of handing the continuation of our program to another party, we could expect it to return us a capability to know when its task finishes, and then our code could decide what to do next?

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1861-1862 | Aggiunto in data sabato 19 maggio 2018 13:43:48</sup></p>

* But what if we could uninvert that inversion of control? What if instead of handing the continuation of our program to another party, we could expect it to return us a capability to know when its task finishes, and then our code could decide what to do next?

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1861-1862 | Aggiunto in data sabato 19 maggio 2018 13:49:17</sup></p>

* But what if we could uninvert that inversion of control? What if instead of handing the continuation of our program to another party, we could expect it to return us a capability to know when its task finishes, and then our code could decide what to do next?

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1861-1862 | Aggiunto in data sabato 19 maggio 2018 13:49:26</sup></p>

* This paradigm is called Promises.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1863-1863 | Aggiunto in data sabato 19 maggio 2018 13:49:32</sup></p>

* “immediately” means in terms of the Job queue behavior (see Chapter 1), not in the strictly synchronous now sense.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1866-1867 | Aggiunto in data sabato 19 maggio 2018 13:58:30</sup></p>

* other words, once my future value was ready, I exchanged my value-promise for the value itself.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1883-1884 | Aggiunto in data sabato 19 maggio 2018 14:11:01</sup></p>

* future values: they can either indicate a success or failure.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1886-1887 | Aggiunto in data sabato 19 maggio 2018 14:11:35</sup></p>

* Note: In code, things are not quite as simple, because metaphorically the order number may never be called, in which case we’re left indefinitely in an unresolved state. We’ll

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1888-1889 | Aggiunto in data sabato 19 maggio 2018 14:12:40</sup></p>

* Note: In code, things are not quite as simple, because metaphorically the order number may never be called, in which case we’re left indefinitely in an unresolved state.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 1888-1889 | Aggiunto in data sabato 19 maggio 2018 14:12:48</sup></p>

* The engine stores values in implementation-dependent ways, and may very well not store them in some object container. What is stored in the container are these property names, which act as pointers (technically, references) to where the values are stored.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11444-11446 | Aggiunto in data mercoledì 9 maggio 2018 19:09:02</sup></p>

* To access the value at the location a in myObject, we need to use either the . operator or the [ ] operator.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11447-11450 | Aggiunto in data mercoledì 9 maggio 2018 19:09:25</sup></p>

* The myObject[..] property access syntax we just described is useful if you need to use a computed expression value as the key name, like myObject[prefix + name]. But that’s not really helpful when declaring objects using the object-literal syntax.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11469-11471 | Aggiunto in data mercoledì 9 maggio 2018 19:11:00</sup></p>

* Symbols, which we will not be covering in detail in this book. In short, they’re a new primitive data type which has an opaque unguessable value (technically a string value). You will be strongly discouraged from working with the actual value of a Symbol (which can theoretically be different between different JS engines), so the name of the Symbol, like Symbol.Something (just a made up name!), will be what you use:

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11476-11481 | Aggiunto in data mercoledì 9 maggio 2018 19:13:07</sup></p>

* Una specie di alias?

<p style="text-align: right;"><sup>La tua nota alla posizione 11478 | Aggiunto in data mercoledì 9 maggio 2018 19:13:48</sup></p>

* interestingly. Technically, functions never “belong” to objects, so saying that a function that just happens to be accessed on an object reference is automatically a “method” seems a bit of a stretch of semantics.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11486-11487 | Aggiunto in data mercoledì 9 maggio 2018 19:16:48</sup></p>

* Arrays assume numeric indexing, which means that values are stored in locations, usually called indices, at non-negative integers, such as 0 and 42.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11518-11520 | Aggiunto in data mercoledì 9 maggio 2018 19:21:25</sup></p>

* Arrays are objects, so even though each index is a positive integer,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11522-11523 | Aggiunto in data mercoledì 9 maggio 2018 19:21:43</sup></p>

* Arrays are objects, so even though each index is a positive integer, you can also add properties onto the array:

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11522-11523 | Aggiunto in data mercoledì 9 maggio 2018 19:21:52</sup></p>

* All is object

<p style="text-align: right;"><sup>La tua nota alla posizione 11523 | Aggiunto in data mercoledì 9 maggio 2018 19:22:11</sup></p>

* careful: If you try to add a property to an array, but the property name looks like a number, it will end up instead as a numeric index (thus modifying the array contents):

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11529-11530 | Aggiunto in data mercoledì 9 maggio 2018 19:23:56</sup></p>

* that objects which are JSON-safe (that is, can be serialized to a JSON string and then re-parsed to an object with the same structure and values) can easily be duplicated with: var newObj = JSON.parse( JSON.stringify( someObj ) );

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11554-11557 | Aggiunto in data mercoledì 9 maggio 2018 19:29:41</sup></p>

* ES6 has now defined Object.assign(..) for this task. Object.assign(..) takes a target object

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11558-11560 | Aggiunto in data mercoledì 9 maggio 2018 19:30:16</sup></p>

* The ability for you to change the value of a property is controlled by writable.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11587-11588 | Aggiunto in data mercoledì 9 maggio 2018 19:43:03</sup></p>

* There’s a nuanced exception to be aware of: even if the property is already configurable:false, writable can always be changed from true to false without error, but

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11611-11613 | Aggiunto in data mercoledì 9 maggio 2018 19:45:00</sup></p>

* Another thing configurable:false prevents is the ability to use the delete operator to remove an existing property.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11614-11616 | Aggiunto in data mercoledì 9 maggio 2018 19:45:33</sup></p>

* It’s important to note that all of these approaches create shallow immutability. That is, they affect only the object and its direct property characteristics. If an object has a reference to another object (array, object, function, etc), the contents of that object are not affected, and remain mutable.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11637-11639 | Aggiunto in data mercoledì 9 maggio 2018 20:24:56</sup></p>

* When you define a property to have either a getter or a setter or both, its definition becomes an “accessor descriptor” (as opposed to a “data descriptor”).

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11714-11716 | Aggiunto in data mercoledì 9 maggio 2018 22:40:37</sup></p>

* We can ask an object if it has a certain property without asking to get that property’s value:

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11747-11747 | Aggiunto in data mercoledì 9 maggio 2018 22:50:35</sup></p>

* ("a" in myObject);

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11748-11749 | Aggiunto in data mercoledì 9 maggio 2018 22:50:51</sup></p>

* myObject.hasOwnProperty( "a" ); // true

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11750-11750 | Aggiunto in data mercoledì 9 maggio 2018 22:51:00</sup></p>

* This difference is important to note with respect to arrays, as the temptation to try a check like 4 in [2, 4, 6] is strong,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11764-11766 | Aggiunto in data mercoledì 9 maggio 2018 23:00:40</sup></p>

* JavaScript actually has classes? Plain and simple: No.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 11948-11949 | Aggiunto in data giovedì 10 maggio 2018 16:13:29</sup></p>

* The top-end of every normal [[Prototype]] chain is the built-in Object.prototype.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12280-12281 | Aggiunto in data venerdì 11 maggio 2018 20:05:48</sup></p>

* Some utilities found here you may be familiar with include .toString() and .valueOf(). In Chapter 3, we introduced another: .hasOwnProperty(..). And yet another function on Object.prototype you may not be familiar with, but which we’ll address later in this chapter, is .isPrototypeOf(..).

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12284-12287 | Aggiunto in data venerdì 11 maggio 2018 20:06:16</sup></p>

* shadowing. The foo property directly on myObject shadows any foo property which appears higher in the chain,

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12301-12303 | Aggiunto in data venerdì 11 maggio 2018 20:07:48</sup></p>

* If a foo is found higher on the [[Prototype]] chain, but it’s marked as read-only

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12313-12314 | Aggiunto in data venerdì 11 maggio 2018 20:08:33</sup></p>

* the creation of the shadowed property on myObject are disallowed.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12315-12316 | Aggiunto in data venerdì 11 maggio 2018 20:08:42</sup></p>

* If a foo is found higher on the [[Prototype]] chain and it’s a setter (see Chapter 3), then the setter will always be called. No foo will be added to (aka, shadowed on) myObject, nor will the foo setter be redefined.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12318-12321 | Aggiunto in data venerdì 11 maggio 2018 20:09:14</sup></p>

* If you want to shadow foo in cases #2 and #3, you cannot use = assignment, but must instead use Object.defineProperty(..) (see Chapter 3) to add foo to myObject.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12323-12326 | Aggiunto in data venerdì 11 maggio 2018 20:09:41</sup></p>

* If you want to shadow foo in cases #2 and #3, you cannot use = assignment, but must instead use Object.defineProperty(..) (see Chapter 3) to add foo to myObject.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12323-12326 | Aggiunto in data venerdì 11 maggio 2018 20:09:50</sup></p>

* In other words, in JavaScript, it’s most appropriate to say that a “constructor” is any function called with the new keyword in front of it.

<p style="text-align: right;"><sup>La tua evidenziazione alla posizione 12458-12460 | Aggiunto in data martedì 15 maggio 2018 18:24:31</sup></p>

