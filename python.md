<h1>Python Fundamentals I & II </h1>
Topics Covered

 <ul>
 <li>Variables and Data Types</li>
  <li>Conditional Logic</li>
   <li>Lists and Dictionaries</li>
    <li>Functions</li>

 <li>Modules and Debugging</li>
  <li>Object Oriented Programming</li>
   <li>File I/O</li>
    <li>Generators, Iterators and Decorators</li>
     <li>Lambdas and Dates</li>
      <li>Variables and Data Types</li>
       <li>Web Scraping</li>
        
 </ul>
 

<h1>Python History and Installation</h1>
<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Explain what Python is and where it is used</li>
<li>Compare and contrast Python2 and Python3 </li>
<li>List common data types in Python </li>
</ul>

<h3>What is Python?</h3>

<p>Python is a popular programming language that you can use to write server-side code for your web applications. You&#39;re only a Google search away from a number of different descriptions of Python, but if you&#39;re looking for an overview, a good place to start is the Python website itself. According to the <a target="_blank" href="https://www.python.org/about/">about</a> page, Python is &quot;powerful... and fast; plays well with others; runs everywhere; is friendly &amp; easy to learn; is Open.&quot;</p>

<p>In 2008, a new version of Python (3.0) was released. Python 3 is the future of the language and is what we will be learning in this class. Not all libraries are compatible with Python 3, but that will change shortly and should not be an issue for your learning. You can read more about the differences <a target="_blank" href="https://wiki.python.org/moin/Python2orPython3">here</a>.</p>

<p>Python is an extremely versatile language and is used by some of the largest companies in the world in multiple fields. It&#39;s beginner-friendly and has a welcoming community and set of standards around writing code in a &quot;Pythonic&quot; way. </p>

<p>We will be using Python 3, so make sure to download it <a target="_blank" href="https://www.python.org/downloads/">here</a>. Once you have downloaded Python 3, your next step is to be sure that you have the package manager for Python 3 installed too. The package manager for Python 3 is called <code>pip3</code>, and it&#39;s what you&#39;ll be using to install any external Python 3 libraries. </p>

<p>To determine whether or not you&#39;ve got <code>pip3</code> installed, type <code>pip3</code> into the terminal. If you see that the command is not found, follow instructions <a target="_blank" href="http://stackoverflow.com/questions/20082935/how-to-install-pip-for-python3-on-mac-os-x">here</a> to install it.</p>

<h3>Some guiding principles in Python</h3>

<p>If you type <code>python3</code> into the terminal and type in <code>import this</code> you can see the guiding principles behind the language. Adhering to these principles will help you write more &quot;Pythonic&quot; code (we will see lots of examples of what that looks like). To exit the Python REPL you can type <code>quit()</code>.</p>

<p>In Python there is something called <code>PEP</code> or <code>Python Enhancement Proposals</code>. Each proposal is simply a document, which can cover new features for the language, style guides, and more. Each proposal has a number that is assigned by the PEP editors, and once a proposal is accepted by the community, it is never changed. You can read more about them <a target="_blank" href="https://www.python.org/dev/peps/">here</a>.</p>

<p>One of the most important <code>PEP</code>s is <code>PEP8</code>, which is a style guide for Python. This guide was written by the creators of the language and is widely accepted as the standard for writing Python code. You can read more about it <a target="_blank" href="https://www.python.org/dev/peps/pep-0008/#indentation">here</a>. If you would like to follow PEP8 rules aggressively you can install the linter for PEP8 with Sublime by installing the <code>SublimeLinter-PEP8</code> package. </p>

<p>If you&#39;d like to read through the entire style guide, you can find it <a target="_blank" href="https://www.python.org/dev/peps/pep-0008/">here</a>.</p>

<h3>Installing a linter for Python</h3>

<p>If <code>PEP8</code> is a little much for you just starting out, there are other linters that are a bit more forgiving. One is <code>Pyflakes</code>, which you can install as follows: in Sublime, press <code>Command + Shift + P</code>, type in <code>SublimeLiner-pyflakes</code>, and press <code>enter</code>. This linter is quite helpful when you first start working in Python and will help you identify issues with indentation, scoping, and other general syntax issues.</p>

<h3>Data Types in Python</h3>

<p>Python has quite a few native datatypes. We&#39;ll provide an overview of a few of the more common ones. For a complete list of the built-in types, check out the <a target="_blank" href="https://docs.python.org/3/library/stdtypes.html">docs</a>. You can also find a list of even more data types available in Python <a target="_blank" href="https://docs.python.org/3/library/datatypes.html">here</a>.</p>

<ul>
<li><strong>Booleans</strong> - As with many other programming languages, there are two booleans in Python: <code>True</code> and <code>False</code> (be mindful of the capitalization).</li>
<li><strong>Numbers</strong> - There are a number (pun intended) of different number types in Python. These include integers (4, 1, -10, etc.), floats (1.3, -2.9, etc), and more.</li>
<li><strong>Strings</strong> - Strings are sequences of Unicode characters, like &quot;hi&quot;, &quot;bye&quot;, and &quot;I love strings!&quot;</li>
<li><strong>Lists</strong> - Lists are ordered sequences of values. The values are comma-separated and in between square brackets. Compared to a language like JavaScript, a list is very similar to an array. Here&#39;s an example of what a list might look like: <code>[1, 2, 3, &quot;the end&quot;]</code>.</li>
<li><strong>Tuples</strong> - Tuples are very similar to lists, but they have one crucial difference. With a list, you can always reassign a value somewhere in the list. However, once you set values in a tuple, you can&#39;t change them. We say that tuples are <em>immutable</em>, as opposed to lists, which are <em>mutable</em>. A tuple uses parentheses rather than brackets: <code>(4, 2, 1)</code> is an example of a tuple.</li>
<li><strong>Sets</strong> - Sets are also similar to lists, but have a couple of big differences. One is that sets don&#39;t keep track of duplicate values: they only store <em>unique</em> values. The second difference is that unlike lists, whose elements are ordered by index, sets don&#39;t impose any order on the elements inside of them. You can think of a set as simply an unordered collection of distinct values. Here&#39;s an example of a set: <code>set(&quot;a&quot;, &quot;b&quot;, &quot;c&quot;)</code>.</li>
<li><strong>Dictionaries</strong> - A dictionary is an unordered collection of key-value pairs. This data type exists in other programming languages, but often goes by other names. For example, a dictionary is similar to a hash in Ruby, or an object in JavaScript. Here&#39;s an example of a dictionary: <code>{&quot;key&quot;: &quot;value&quot;, &quot;a&quot;: 0}</code>.</li>
</ul>

<p>We&#39;ll learn much more about these data types in the coming chapters!</p>

<h3>Running Python Code</h3>

<p>To get started with a Python <code>REPL</code>, which is where you will be writing your code, make sure python is installed and anywhere in the terminal, type in <code>python3</code>. To exit the <code>REPL</code> you can type <code>quit()</code> or press <code>control + d</code>.</p>

<p>If you find it easier to use, you can check out <a target="_blank" href="https://repl.it/languages/python3">repl.it</a> for Python3 and start here. To run your code you can click the run button (or use the keyboard shortcut you see when you hover over the button). </p>

<p>If you would like to write larger Python files, you can save them as <code>.py</code> files. Let&#39;s imagine that you create a file called <code>first.py</code>. If you want to run that file, you have to make sure you are in the same directory (folder) where the file is saved. To run the file, make sure you are in the Terminal/Command Line and run <code>python3 first.py</code>. If you are not comfortable in the Terminal, check out our free online courses on Terminal and UNIX!</p>

<p>        When you're ready, move on to Variables and Primitives</p>

<h1> Variables and Primitives. </h1>
 <h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Define variables in Python</li>
<li>Explain the difference between ASCII and Unicode</li>
<li>Use basic methods to manipulate strings in Python</li>
</ul>

<h3>Variables</h3>

<p>Declaring a variable in Python is quite easy; just use <code>=</code> to assign a value to a variable. If you want to indicate an absence of value, you can assign a variable to the value <code>None</code>.</p>
<div class="CodeRay">
  <div class="code"><pre>a = <span class="integer">1</span>
b = <span class="string"><span class="delimiter">&quot;</span><span class="content">YOLO</span><span class="delimiter">&quot;</span></span>
nothing = <span class="predefined-constant">None</span>
</pre></div>
</div>

<p>In Python you can also do multiple assignment with variables separated by a comma. This is quite common with Python so make sure to try this out. Here&#39;s a basic example:</p>
<div class="CodeRay">
  <div class="code"><pre>a,b = <span class="integer">1</span>,<span class="integer">2</span>
a <span class="comment"># 1</span>
b <span class="comment"># 2</span>
</pre></div>
</div>

<p>By convention, variable names should be written in <code>snake_case</code>. This means that all words should be lowercase, and words should be separated by an underscore. This is a very strong convention in Python, so you should get into the habit as quickly as possible!</p>
<div class="CodeRay">
  <div class="code"><pre>myVariable = <span class="integer">3</span> <span class="comment"># Get outta here, this isn't JavaScript!</span>
my_variable = <span class="integer">3</span> <span class="comment"># much better</span>
</pre></div>
</div>

<h3>Types in Python</h3>

<p>As we mentioned in the last chapter, Python has quite a few built in data types, including booleans, numeric types (int, float), strings, tuples, lists, dictionaries, and many more. We can see the type of an object using the built in <code>type</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="predefined">type</span>(<span class="predefined-constant">False</span>) <span class="comment"># bool</span>
<span class="predefined">type</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">nice</span><span class="delimiter">&quot;</span></span>) <span class="comment"># str</span>
<span class="predefined">type</span>({}) <span class="comment"># dict</span>
<span class="predefined">type</span>([]) <span class="comment"># list</span>
<span class="predefined">type</span>(()) <span class="comment"># tuple</span>
<span class="predefined">type</span>(<span class="predefined-constant">None</span>) <span class="comment"># NoneType</span>
</pre></div>
</div>

<h3>Strings in Python</h3>

<p>In Python 2 strings, are stored internally as 8 bit ASCII. But in Python 3, all strings are represented in Unicode. </p>

<p><strong>Uh, what?</strong></p>

<p>Before we talk about methods on strings in Python, let&#39;s learn a little bit about the history of character encodings. If you would like a longer description, feel free to read <a target="_blank" href="http://www.diveintopython3.net/strings.html">this</a> excellent article.</p>

<p>When we as humans see text on a computer screen, we are viewing something quite different than what a computer processes. Remember that computers deal with bits and bytes, so we need a way to <em>encode</em> (or <em>map</em>) characters to something a computer can work with. In 1968, the American Standard Code for Information Interchange (or ASCII) was standardized as a character encoding. ASCII defined codes for characters ranging from 0 to 127. </p>

<p>Why this range? Remember that computers work in base 2 or binary, so each bit represents a power of two. This means that 7 bits can get us <code>2^7 = 128</code> different binary numbers; since each bit can equal <code>0</code> or <code>1</code>, with <code>7</code> bits we can represent all numbers from <code>0000000</code> up to  <code>1111111</code>. With ASCII, we can then map each of these numbers to a distinct character. Since there are only 26 letters in the alphabet (52 if you care about the distinction between upper and lower case), plus a handful of digits and punctuation characters, ASCII should more than cover our needs, right?</p>

<p>ASCII was a great start, but issues arose when non English characters like <code>é</code> or <code>ö</code> could not be processed and would just be converted to <code>e</code> and <code>o</code>. In the 1980s, computers were 8-bit machines which meant that bytes now held 8 bits. The highest binary number we could obtain on these machines was <code>11111111</code> or  <code>2^0 + 2^1 + 2^2 + 2^3 + 2^4 + 2^5 + 2^6 + 2^7</code>, or <code>255</code>. Different machines now used the values of 128 to 255 for accented characters, but there was not a standard that emerged until the International Standards Organization (or ISO) emerged. </p>

<p>Even with an additional <code>128</code> characters, we started running into lots of issues once the web grew. Languages with completely different character sets like Russian, Chinese, Arabic, and many more had to be encoded in completely different character sets, causing a nightmare when trying to deliver a single text file with multiple character sets. </p>

<p>In the 1980s, a new encoding called <code>Unicode</code> was introduced. Unicode&#39;s mission was to encode all possible characters and still be backward compatible with ASCII. The most popular character encoding that is dominant on the web now is <code>UTF-8</code>, which uses <code>8-bit</code> code units, but with a variable length to ensure that all sorts of characters can be encoded. </p>

<p>TL;DR: in Python3, strings are Unicode by default. </p>

<h3>String Methods</h3>

<p>Python contains quite a few helpful string methods; here are a few. Try running these in a REPL to see what they do!</p>

<p>Let&#39;s start with a simple variable:</p>
<div class="CodeRay">
  <div class="code"><pre>string = <span class="string"><span class="delimiter">&quot;</span><span class="content">this Is nIce</span><span class="delimiter">&quot;</span></span>
</pre></div>
</div>

<h4>Upper</h4>

<p>To convert every character to upper-case we can use the <code>upper</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.upper() <span class="comment"># 'THIS IS NICE'</span>
</pre></div>
</div>

<h4>Lower</h4>

<p>To convert every character to lower-case we can use the <code>lower</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.lower() <span class="comment"># 'this is nice'</span>
</pre></div>
</div>

<h4>Capitalize</h4>

<p>To convert the first character in a string to upper-case and everything else to lower-case we can use the <code>capitalize</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.capitalize() <span class="comment"># 'This is nice'</span>
</pre></div>
</div>

<h4>Title</h4>

<p>To convert every first character in a string to upper-case and everything else to lower-case we can use the <code>title</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.title() <span class="comment"># 'This Is Nice'</span>
</pre></div>
</div>

<h4>Find</h4>

<p>To find a subset of characters in a string we can use the <code>find</code> method. This will return the index at which the first match occurs. If the character/characters is/are not found, <code>find</code> will return <code>-1</code></p>
<div class="CodeRay">
  <div class="code"><pre>
instructor = <span class="string"><span class="delimiter">'</span><span class="content">elie</span><span class="delimiter">'</span></span>
instructor.find(<span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>) <span class="comment"># 0</span>
instructor.find(<span class="string"><span class="delimiter">'</span><span class="content">E</span><span class="delimiter">'</span></span>) <span class="comment"># -1 it IS case sensitive!</span>

string.find(<span class="string"><span class="delimiter">&quot;</span><span class="content">i</span><span class="delimiter">&quot;</span></span>) <span class="comment"># 2, since the character &quot;i&quot; is at index 2</span>
string.find(<span class="string"><span class="delimiter">'</span><span class="content">Tim</span><span class="delimiter">'</span></span>) <span class="comment"># -1 </span>
</pre></div>
</div>

<h4>isalpha</h4>

<p>To see if all characters are alphabetic we can use the <code>isalpha</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.isalpha() <span class="comment"># False</span>
string[<span class="integer">0</span>].isalpha() <span class="comment"># True</span>
</pre></div>
</div>

<h4>isspace</h4>

<p>To see if a character or all characters are empty spaces, we can use the <code>isspace</code> function</p>
<div class="CodeRay">
  <div class="code"><pre>string.isspace() <span class="comment"># False</span>
string[<span class="integer">0</span>].isspace() <span class="comment"># False</span>
string[<span class="integer">4</span>].isspace() <span class="comment"># True</span>
</pre></div>
</div>

<h4>islower</h4>

<p>To see if a character or all characters are lower-cased , we can use the <code>islower</code> function (there is also a function, which does the inverse called <code>isupper</code>)</p>
<div class="CodeRay">
  <div class="code"><pre>string.islower() <span class="comment"># False</span>
string[<span class="integer">0</span>].islower() <span class="comment"># True</span>
string[<span class="integer">5</span>].islower() <span class="comment"># False</span>
string.lower().islower() <span class="comment"># True</span>
</pre></div>
</div>

<h4>istitle</h4>

<p>To see if a string is a &quot;title&quot; (first character of each word is capitalized), we can use the <code>istitle</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.istitle() <span class="comment"># False</span>
string.title().istitle() <span class="comment"># True</span>

<span class="string"><span class="delimiter">&quot;</span><span class="content">not Awesome Sauce</span><span class="delimiter">&quot;</span></span>.istitle() <span class="comment"># False</span>
<span class="string"><span class="delimiter">&quot;</span><span class="content">Awesome Sauce</span><span class="delimiter">&quot;</span></span>.istitle() <span class="comment"># True</span>

</pre></div>
</div>

<h4>endswith</h4>

<p>To see if a string ends with a certain set of characters we can use the <code>endswith</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="string"><span class="delimiter">&quot;</span><span class="content">string</span><span class="delimiter">&quot;</span></span>.endswith(<span class="string"><span class="delimiter">'</span><span class="content">g</span><span class="delimiter">'</span></span>) <span class="comment"># True</span>
<span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>.endswith(<span class="string"><span class="delimiter">'</span><span class="content">foo</span><span class="delimiter">'</span></span>) <span class="comment"># False</span>
</pre></div>
</div>

<h4>partition</h4>

<p>To partition a string based on a certain character, we can use the <code>partition</code> function.</p>
<div class="CodeRay">
  <div class="code"><pre>string.partition(<span class="string"><span class="delimiter">'</span><span class="content">i</span><span class="delimiter">'</span></span>) <span class="comment"># what's the type of what you get back?</span>
<span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>.partition(<span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>) <span class="comment"># ('aw', 'e', 'some')</span>
</pre></div>
</div>

<h3>Formatting strings with <code>format</code></h3>

<p>One of the most common string methods you&#39;ll use is the <code>format</code> method. This is a powerful method that can do all kinds of string manipulation (see here for an entire <a target="_blank" href="https://pyformat.info/#simple">book</a> on it), but it&#39;s most commonly just used to pass varaibles into strings. In general this is preferred over string concatenation, which can quickly get cumbersome if you&#39;re mixing a lot of variables with strings. For example:</p>
<div class="CodeRay">
  <div class="code"><pre>first_name = <span class="string"><span class="delimiter">&quot;</span><span class="content">Matt</span><span class="delimiter">&quot;</span></span>
last_name = <span class="string"><span class="delimiter">&quot;</span><span class="content">Lane</span><span class="delimiter">&quot;</span></span>
city = <span class="string"><span class="delimiter">&quot;</span><span class="content">San Francisco</span><span class="delimiter">&quot;</span></span>
mood = <span class="string"><span class="delimiter">&quot;</span><span class="content">great</span><span class="delimiter">&quot;</span></span>

greeting = <span class="string"><span class="delimiter">&quot;</span><span class="content">Hi, my name is </span><span class="delimiter">&quot;</span></span> + first_name + <span class="string"><span class="delimiter">&quot;</span><span class="content"> </span><span class="delimiter">&quot;</span></span> + last_name + <span class="string"><span class="delimiter">&quot;</span><span class="content">, I live in </span><span class="delimiter">&quot;</span></span> + city + <span class="string"><span class="delimiter">&quot;</span><span class="content"> and I feel </span><span class="delimiter">&quot;</span></span> + mood + <span class="string"><span class="delimiter">&quot;</span><span class="content">.</span><span class="delimiter">&quot;</span></span>
greeting <span class="comment"># 'Hi, my name is Matt Lane, I live in San Francisco and I feel great.'</span>
</pre></div>
</div>

<p>Here, the <code>greeting</code> variable looks fine, but all that string concatenation isn&#39;t easy on the eyes. It&#39;s very easy to forget about a <code>+</code> sign, or to forget to separate words with extra whitespace at the beginning and end of our strings.</p>

<p>This is one reason why <code>format</code> is nice. Here&#39;s a refactor:</p>
<div class="CodeRay">
  <div class="code"><pre>greeting = <span class="string"><span class="delimiter">&quot;</span><span class="content">Hi, my name is {} {}, I live in {} and I feel {}.</span><span class="delimiter">&quot;</span></span>.format(first_name, last_name, city, mood)
</pre></div>
</div>

<p>When we call <code>format</code> on a string, we can pass variables into the string! The variables will be passed in order, wherever <code>format</code> finds a set of curly braces.</p>

<p>If the empty curly braces seem a little weird, we can also create variable names and assign them to the values we&#39;re passing in:</p>
<div class="CodeRay">
  <div class="code"><pre>greeting = <span class="string"><span class="delimiter">&quot;</span><span class="content">Hi, my name is {first} {last}, I live in {my_city}, and I feel {my_mood}.</span><span class="delimiter">&quot;</span></span>.format(
    first=first_name, 
    last=last_name,
    my_city=city, 
    my_mood=mood
)
</pre></div>
</div>

<p>This approach can be helpful if you want to pass in the same variable multiple times in your string:</p>
<div class="CodeRay">
  <div class="code"><pre>new_greeting = <span class="string"><span class="delimiter">&quot;</span><span class="content">Hi, my name is {name}. My friends call me {name}. You can call me {name}.</span><span class="delimiter">&quot;</span></span>.format(name=first_name)
</pre></div>

When you're ready, move on to  Boolean Logic.

<h1>Boolean Logic.</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Write conditional logic using boolean operators</li>
<li>List examples of falsey values in Python</li>
<li>Use if/else to include conditional logic in your Python code</li>
<li>Explain the difference between <code>==</code> and <code>is</code> in Python</li>
<li>Convert between data types explicitly in Python</li>
</ul>

<h2>Boolean Logic</h2>

<p>An essential part of writing programs is being able to execute code that depends on certain conditions. There are many different examples when you&#39;d want to conditionally execute code. Here are just a few:</p>

<ul>
<li>You want the navigation bar on your website to look different based on whether or not someone is logged in</li>
<li>If someone enters their password incorrectly, you want to let them know; otherwise, you want to log them in</li>
<li>You&#39;re building a tic-tac-toe game, and want to know whether it&#39;s X&#39;s turn or O&#39;s turn</li>
<li>You&#39;re building a social network and want to keep person A from seeing person B&#39;s profile unless the two of them are friends</li>
</ul>

<p>And so on, and so on. It&#39;s very hard to write any kind of interesting software without making use of conditionals and boolean logic.</p>

<p>So let&#39;s talk about how to write conditional logic in Python. To do so, we&#39;ll make use of booleans (<code>True</code> and <code>False</code>), along with <code>if</code> statements.</p>

<h3>Conditionals</h3>

<p>Like many other programming languages, Python has conditionals with <code>if/else</code> statements. One difference with Python, however, is that it does not use the <code>else if</code> construct for chaining multiple conditions together. Instead, Python uses the keyword <code>elif</code> (short for <code>else if</code>). Note also that Python does not require parenthesis around conditions, but each condition must end with a <code>:</code>. If you forget the colon (a very common mistake when you&#39;re first learning Python!), you&#39;ll get a <code>SyntaxError</code>. Change the value of the <code>user</code> variable in the example below.  Try to get each case to print to your console:</p>
<div class="CodeRay">
  <div class="code"><pre>user = <span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>
<span class="keyword">if</span> user == <span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>:
    print(<span class="string"><span class="delimiter">'</span><span class="content">Awesome!</span><span class="delimiter">'</span></span>)
<span class="keyword">elif</span> user == <span class="string"><span class="delimiter">'</span><span class="content">Tom</span><span class="delimiter">'</span></span>:
    print(<span class="string"><span class="delimiter">'</span><span class="content">Cool!</span><span class="delimiter">'</span></span>)
<span class="keyword">else</span>:
    print(<span class="string"><span class="delimiter">'</span><span class="content">Nope!</span><span class="delimiter">'</span></span>)
</pre></div>
</div>

<p>Python also allows you to use words like <code>or</code>, <code>and</code>, and <code>not</code> for comparison</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">if</span> <span class="integer">1</span> &gt; <span class="integer">2</span> <span class="keyword">or</span> <span class="integer">2</span> &gt; <span class="integer">1</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">cool!</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">if</span> <span class="integer">1</span> == <span class="integer">1</span> <span class="keyword">and</span> <span class="integer">2</span> == <span class="integer">2</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">nice!</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">if</span> <span class="keyword">not</span> <span class="predefined-constant">False</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">it is true!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>One nice thing about comparing numbers is that you can string inequalities together without using the <code>and</code> keyword:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">if</span> <span class="integer">1</span> &lt; <span class="integer">2</span> <span class="keyword">and</span> <span class="integer">2</span> &lt; <span class="integer">3</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">this is ok</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">if</span> <span class="integer">1</span> &lt; <span class="integer">2</span> &lt; <span class="integer">3</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">this is better!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>Also, it&#39;s important to understand that the indentation in all of these examples matters tremendously. Indentation is how Python keeps track of what code should be executed conditionally, and which code should always be executed:</p>
<div class="CodeRay">
  <div class="code"><pre>name = <span class="string"><span class="delimiter">&quot;</span><span class="content">Matt</span><span class="delimiter">&quot;</span></span>
<span class="keyword">if</span> name == <span class="string"><span class="delimiter">&quot;</span><span class="content">Matt</span><span class="delimiter">&quot;</span></span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">Your name is Matt</span><span class="delimiter">&quot;</span></span>)
print(<span class="string"><span class="delimiter">&quot;</span><span class="content">Bye!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>In the example above, both messages will be printed. But if you change the name variable to something besides <code>&quot;Matt&quot;</code>, the second print statement will still execute. Because of the indentation, Python knows that the last line is not part of the <code>if</code> statement!</p>

<p>If you forget about indentation, Python will throw an error. Python enforces indentation fairly strongly, but if you make a mistake, it&#39;ll let you know!</p>
<div class="CodeRay">
  <div class="code"><pre>name = <span class="string"><span class="delimiter">&quot;</span><span class="content">Matt</span><span class="delimiter">&quot;</span></span>
<span class="keyword">if</span> name == <span class="string"><span class="delimiter">&quot;</span><span class="content">Matt</span><span class="delimiter">&quot;</span></span>:
print(<span class="string"><span class="delimiter">&quot;</span><span class="content">Your name is Matt</span><span class="delimiter">&quot;</span></span>) <span class="comment"># IndentationError!</span>
</pre></div>
</div>

<h3>Falsey Values in Python</h3>

<p>Python has quite a few falsey values (values that evaluate to <code>False</code> when converted to a boolean). We can check whether a value is falsey by passing it into the <code>bool</code> function!  All of the following examples evaluate to false when converted to a boolean.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># False</span>
<span class="predefined">bool</span>(<span class="predefined-constant">False</span>)

<span class="comment"># 0</span>
<span class="predefined">bool</span>(<span class="integer">0</span>)

<span class="comment"># None</span>
<span class="predefined">bool</span>(<span class="predefined-constant">None</span>)

<span class="comment"># Empty string</span>
<span class="predefined">bool</span>(<span class="string"><span class="delimiter">&quot;</span><span class="delimiter">&quot;</span></span>)

<span class="comment"># Empty list</span>
<span class="predefined">bool</span>([])

<span class="comment"># Empty tuple</span>
<span class="predefined">bool</span>(())

<span class="comment"># Empty dictionary</span>
<span class="predefined">bool</span>({})

<span class="comment"># Empty set</span>
<span class="predefined">bool</span>(<span class="predefined">set</span>())
</pre></div>
</div>

<h3>Comparison: <code>is</code> versus <code>==</code></h3>

<p>Everything in Python is an object with an id. To see if two objects have the same id, you can use the <code>is</code> operator. You can also inspect an object&#39;s id directly using the <code>id</code> function.</p>

<ul>
<li><code>is</code> operator (compares id)</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>a = <span class="integer">1</span> 
b = a 
b <span class="keyword">is</span> a <span class="comment"># True</span>
b = <span class="integer">2</span> 
a <span class="keyword">is</span> b <span class="comment"># False</span>
<span class="predefined">id</span>(a) <span class="comment"># should give you a number</span>
</pre></div>
</div>

<p>If you just want to check whether two objects have the same <em>value</em>, you can use the <code>==</code> comparator. In general, it&#39;s probably best to use <code>==</code> for comparison, unless you know that you&#39;re trying to determine whether two objects have the same id (i.e. they are the same object in memory).</p>
<div class="CodeRay">
  <div class="code"><pre>list1 = [<span class="integer">1</span>, <span class="integer">2</span>]
list2 = [<span class="integer">1</span>, <span class="integer">2</span>]
list3 = list1

list1 <span class="keyword">is</span> list3 <span class="comment"># True</span>
list1 <span class="keyword">is</span> list2 <span class="comment"># False</span>

list1 == list3 <span class="comment"># True</span>
list1 == list2 <span class="comment"># True</span>
</pre></div>
</div>

<h3>Gathering user input</h3>

<p>Before we move on to the exercises, there&#39;s one more function you should know about. It is very common in command line programs to prompt the user for information. In Python, this function is called <code>input</code>. Here&#39;s an example:</p>
<div class="CodeRay">
  <div class="code"><pre>name = <span class="predefined">input</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">What is your name? </span><span class="delimiter">&quot;</span></span>)
<span class="comment"># you can now type anything and it will be saved into the name variable</span>
</pre></div>
</div>

<h3>pass</h3>

<p>Since Python is very sensitive to indentation, there may be situations where you need to place indented code, but do not want to run anything. In this case, the <code>pass</code> keyword must be used.</p>

When you're ready, move on to Boolean Logic Exercise </p>

<h1>Boolean Logic Exercises.</h1>

<p>Complete the exercises below by writing an expression in Python to answer the question:</p>

<ol>
<li><p>Declare a variable called <code>first</code> and assign it to the value <code>&quot;Hello World&quot;</code>.</p></li>
<li><p>Write a comment that says <code>&quot;This is a comment.&quot;</code></p></li>
<li><p>Log a message to the terminal that says <code>&quot;I AM A COMPUTER!&quot;</code></p></li>
<li><p>Write an if statement that checks if <code>1</code> is less than <code>2</code> and if <code>4</code> is greater than <code>2</code>. If it is, show the message <code>&quot;Math is fun.&quot;</code>`</p></li>
<li><p>Assign a variable called <code>nope</code> to an absence of value.</p></li>
<li><p>Use the language&#39;s &quot;and&quot; boolean operator to combine the language&#39;s &quot;true&quot; value with its &quot;false&quot; value.</p></li>
<li><p>Calculate the length of the string <code>&quot;What&#39;s my length?&quot;</code></p></li>
<li><p>Convert the string <code>&quot;i am shouting&quot;</code> to uppercase.</p></li>
<li><p>Convert the string <code>&quot;1000&quot;</code> to the number <code>1000</code>.</p></li>
<li><p>Combine the number <code>4</code> with the string <code>&quot;real&quot;</code> to produce <code>&quot;4real&quot;</code>.</p></li>
<li><p>Record the output of the expression <code>3 * &quot;cool&quot;</code>.</p></li>
<li><p>Record the output of the expression <code>1 / 0</code>.</p></li>
<li><p>Determine the type of <code>[]</code>. </p></li>
<li><p>Ask the user for their name, and store it in a variable called <code>name</code>.</p></li>
<li><p>Ask the user for a number. If the number is negative, show a message that says <code>&quot;That number is less than 0!&quot;</code> If the number is positive, show a message that says <code>&quot;That number is greater than 0!&quot;</code> Otherwise, show a message that says <code>&quot;You picked 0!</code>.</p></li>
<li><p>Find the index of <code>&quot;l&quot;</code> in <code>&quot;apple&quot;</code>.</p></li>
<li><p>Check whether <code>&quot;y&quot;</code> is in <code>&quot;xylophone&quot;</code>.</p></li>
<li><p>Check whether a string called <code>my_string</code> is all in lowercase.</p></li>
</ol>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_1_solutions/blob/master/python_boolean_logic/solutions.md">here</a>.</p>

<h1> List Basics.</h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Define what a list is in Python</li>
<li>Access and reassign values in a list</li>
<li>Operate on lists using common built-in methods</li>
<li>Create copies of lists and strings using slices</li>
</ul>

<h3>Lists</h3>

<p>Lists in Python are simply collections of elements. They can be as long as you want, and the individual elements can have the same type or not:</p>
<div class="CodeRay">
  <div class="code"><pre>number_list = [<span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>]
string_list = [<span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">b</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">c</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">d</span><span class="delimiter">&quot;</span></span>]
kitchen_sink_list = [<span class="integer">4</span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">yo</span><span class="delimiter">&quot;</span></span>, <span class="predefined-constant">None</span>, <span class="predefined-constant">False</span>, <span class="predefined-constant">True</span>, [<span class="string"><span class="delimiter">&quot;</span><span class="content">another</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">list</span><span class="delimiter">&quot;</span></span>]]
</pre></div>
</div>

<p>To access an element in a list, we use bracket notation and pass in the index we&#39;re interested in. Lists in Python use a zero-based index:</p>
<div class="CodeRay">
  <div class="code"><pre>my_list = [<span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>, <span class="integer">1</span>, <span class="predefined-constant">True</span>]
my_list[<span class="integer">0</span>] <span class="comment"># &quot;a&quot;</span>
my_list[<span class="integer">2</span>] <span class="comment"># True</span>
my_list[<span class="integer">3</span>] <span class="comment"># IndexError</span>
</pre></div>
</div>

<p>Note that if you try to access an element with an invalid index, Python will give you an error.</p>

<p>We can also reassign values in lists using <code>=</code>:</p>
<div class="CodeRay">
  <div class="code"><pre>my_list = [<span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>, <span class="integer">1</span>, <span class="predefined-constant">True</span>]
my_list[<span class="integer">2</span>] = <span class="predefined-constant">False</span>
my_list <span class="comment"># [&quot;a&quot;, 1, False]</span>
</pre></div>
</div>

<p>In addition to getting and setting values in lists, there are a number of built-in methods you can use. Here are some more ones (in alphabetical order):</p>

<h4><code>append</code></h4>

<p>Adds a value to the end of a list:</p>
<div class="CodeRay">
  <div class="code"><pre>my_list = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>]
my_list.append(<span class="integer">10</span>)
my_list <span class="comment"># [1,2,3,10]</span>
</pre></div>
</div>

<h4><code>clear</code></h4>

<p>Removes all the values in a list:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>]
l.clear()
l <span class="comment"># []</span>
</pre></div>
</div>

<h4><code>copy</code></h4>

<p>Makes a copy of a list:</p>
<div class="CodeRay">
  <div class="code"><pre>l = []
l.append(<span class="integer">2</span>)
l.append(<span class="integer">3</span>)
l.append(<span class="integer">4</span>)
l <span class="comment"># [2, 3, 4]</span>
z = l.copy()
z <span class="comment"># [2, 3, 4]</span>
l <span class="comment"># [2, 3, 4]</span>
z.remove(<span class="integer">3</span>)
z <span class="comment"># [2, 4]</span>
l <span class="comment"># [2, 3, 4]</span>
</pre></div>
</div>

<h4><code>count</code></h4>

<p>Counts how many times an item appears in a list:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">5</span>,<span class="integer">5</span>,<span class="integer">5</span>]
l.count(<span class="integer">1</span>) <span class="comment"># 1</span>
l.count(<span class="integer">5</span>) <span class="comment"># 4</span>
</pre></div>
</div>

<h4><code>extend</code></h4>

<p>Appends another list and flattens the appended list (so there is not a list inside of a list):</p>
<div class="CodeRay">
  <div class="code"><pre>
l = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>]
l.append([<span class="integer">4</span>])
l <span class="comment"># [1,2,3,[4]]</span>

l.extend([<span class="integer">5</span>,<span class="integer">6</span>,<span class="integer">7</span>])
l <span class="comment"># [1,2,3,[4],5,6,7] </span>

</pre></div>
</div>

<h4><code>index</code></h4>

<p>Returns the index at which a value is found. If the value is not found, <code>index</code> returns a <code>ValueError</code>:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">4</span>,<span class="integer">8</span>,<span class="integer">6</span>,<span class="integer">4</span>]
l.index(<span class="integer">8</span>) <span class="comment"># 1</span>
l.index(<span class="integer">4</span>) <span class="comment"># 0 - it only finds the index of the first matching element</span>
l.index(<span class="integer">12</span>) <span class="comment"># ValueError</span>
</pre></div>
</div>

<h4><code>insert</code></h4>

<p>Takes in an index and a value, and inserts the value at the given index:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">4</span>,<span class="integer">6</span>,<span class="integer">8</span>]
l.insert(<span class="integer">2</span>,<span class="string"><span class="delimiter">'</span><span class="content">awesome</span><span class="delimiter">'</span></span>) <span class="comment"># insert 'awesome' at index 2</span>
l <span class="comment"># [4,6,'awesome',8]</span>
</pre></div>
</div>

<h4><code>pop</code></h4>

<p>By default, pop removes the last element from a list. If pop is given an index as an argument, the element at that index is removed. This method returns the element removed:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">3</span>,<span class="integer">4</span>]
l.pop(<span class="integer">0</span>) <span class="comment"># 3</span>
l.pop() <span class="comment"># 4</span>
l.pop() <span class="comment"># IndexError</span>
</pre></div>
</div>

<p>Notice that <code>pop</code> throws an error if you call it on an empty list!</p>

<h4><code>remove</code></h4>

<p>Removes the first occurrence of a value:</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">1</span>]
l.remove(<span class="integer">1</span>)
l <span class="comment"># [2,3,1]</span>
l.remove(<span class="integer">5</span>) <span class="comment"># ValueError</span>
</pre></div>
</div>

<p>Notice that <code>remove</code> throws an error if you try to remove something not in the list.</p>

<h4><code>reverse</code></h4>

<p>Reverses a list in place (i.e. it mutates the original list):</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]
l.reverse()
l <span class="comment"># [4,3,2,1]</span>
</pre></div>
</div>

<h4><code>sort</code></h4>

<p>Sorts the list in place (i.e. it mutates the original list):</p>
<div class="CodeRay">
  <div class="code"><pre>l = [<span class="integer">1</span>,<span class="integer">4</span>,<span class="integer">3</span>,<span class="integer">2</span>]
l.sort()
l <span class="comment"># [1,2,3,4]</span>
</pre></div>
</div>

<h3>Slicing lists</h3>

<p>Slices return portions of a list <strong>or</strong> string. While this seems like a pretty minor concept, there&#39;s actually quite a bit you can do with slices that you might not expect. </p>

<p>The standard syntax for a slice is <code>list[start:end]</code>, or <code>list[start:end:step]</code>. We can also do <code>list[:]</code> to make a copy of a list, or even <code>list[::-1]</code> to make a copy of a reversed list.</p>

<p>Let&#39;s see some examples :</p>
<div class="CodeRay">
  <div class="code"><pre>first_list = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">6</span>]
first_list[<span class="integer">0</span>:<span class="integer">1</span>] <span class="comment"># [1]</span>

<span class="comment"># if a value for end isn't provided, you'll slice to the end of the list</span>
first_list[<span class="integer">1</span>:] <span class="comment"># [2, 3, 4, 5, 6]</span>

<span class="comment"># if a value for start isn't provided, you'll slice from the start of the list</span>
first_list[:<span class="integer">3</span>] <span class="comment"># [1,2,3]</span>

<span class="comment"># get the last element in the list</span>
first_list[-<span class="integer">1</span>] <span class="comment"># 6</span>

<span class="comment"># start from the second to last element in the list</span>
first_list[-<span class="integer">2</span>:] <span class="comment"># [5, 6]</span>

<span class="comment"># There is always more than one way of doing something...</span>
first_list[<span class="integer">4</span>:] == first_list[-<span class="integer">2</span>:] <span class="comment"># True</span>

<span class="comment"># step in the opposite direction</span>
first_list[::-<span class="integer">1</span>] <span class="comment"># [6, 5, 4, 3, 2, 1]</span>

<span class="comment"># step in the opposite direction by two elements</span>
first_list[::-<span class="integer">2</span>] <span class="comment"># [6, 4, 2]</span>
</pre></div>
</div></div>
When you're ready, move on to List Iteration and Comprehension

<h1>List Iteration and Comprehension.</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Iterate through lists and strings </li>
<li>Create and iterate through ranges</li>
<li>Use list comprehension to write concise loops</li>
</ul>

<h3>Iterating over lists and strings</h3>

<p>In Python we have a few ways of iterating over lists and strings. One of the most common types of loops is a <code>for in</code> loop; <code>while</code> loops are also common. Let&#39;s see what those look like.</p>

<h4>for in</h4>

<p>The most common way of iterating over a list is a <code>for in</code> loop. The syntax is <code>for ELEMENT in LIST:</code>. As with <code>if</code> statements, don&#39;t forget about the colon!</p>
<div class="CodeRay">
  <div class="code"><pre>values = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]

<span class="keyword">for</span> val <span class="keyword">in</span> values:
    print(val) 

<span class="comment"># 1</span>
<span class="comment"># 2</span>
<span class="comment"># 3</span>
<span class="comment"># 4</span>

<span class="keyword">for</span> char <span class="keyword">in</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>:
    print(char)

<span class="comment"># a</span>
<span class="comment"># w</span>
<span class="comment"># e</span>
<span class="comment"># s</span>
<span class="comment"># o</span>
<span class="comment"># m</span>
<span class="comment"># e</span>
</pre></div>
</div>

<p>Sometimes you may want to have access to the element&#39;s index in the list as well as the element itself. In this case, you can pass the list into the <code>enumerate</code> function. You&#39;ll need to name two variables in the <code>for</code> loop: the first will refer to the current index, the second will refer to the current element:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">for</span> idx, char <span class="keyword">in</span> <span class="predefined">enumerate</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>):
    print(idx, char)

<span class="comment"># 0 a</span>
<span class="comment"># 1 w</span>
<span class="comment"># 2 e</span>
<span class="comment"># 3 s</span>
<span class="comment"># 4 o</span>
<span class="comment"># 5 m</span>
<span class="comment"># 6 e</span>
</pre></div>
</div>

<h4>while</h4>

<p>You can also do a <code>while</code> loop with Python, but this is a bit less common when iterating:</p>
<div class="CodeRay">
  <div class="code"><pre>i = <span class="integer">0</span>
<span class="keyword">while</span> i &lt; <span class="integer">5</span>:
    print(i)
    i +=<span class="integer">1</span>

<span class="comment"># 0</span>
<span class="comment"># 1</span>
<span class="comment"># 2</span>
<span class="comment"># 3</span>
<span class="comment"># 4</span>
</pre></div>
</div>

<p>If you ever want to move to the next step of the iteration, you can prematurely break out of the current iteration with the the <code>continue</code> keyword. Similarly, you can exit from a loop entirely using the <code>break</code> keyword.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">for</span> num <span class="keyword">in</span> [<span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>]:
    <span class="keyword">if</span> num % <span class="integer">2</span> == <span class="integer">0</span>:
        <span class="keyword">continue</span>
    <span class="keyword">elif</span> num &gt; <span class="integer">5</span>:
        <span class="keyword">break</span>
    print(num)

<span class="comment"># 1</span>
<span class="comment"># 3</span>
<span class="comment"># 5</span>
<span class="comment"># the loop continues before the print statement if num is even,</span>
<span class="comment"># and it ends entirely when num is 6, so the last odd number doesn't get printed.   </span>
</pre></div>
</div>

<h4>range</h4>

<p>In Python we can also create ranges, which represent a range of numbers, with the following syntax: <code>range(start,stop,step)</code>. Note that the range <strong>is not</strong> inclusive.  In other words, <code>range(1,4)</code> will include 1, 2, and 3, but not 4!</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># We can do some pretty cool things with range</span>
(a,b,c,d) = <span class="predefined">range</span>(<span class="integer">4</span>)
a <span class="comment"># 0</span>
b <span class="comment"># 1</span>
c <span class="comment"># 2</span>
d <span class="comment"># 3</span>

<span class="keyword">for</span> num <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">4</span>,<span class="integer">10</span>):
    print(num)

<span class="comment"># 4</span>
<span class="comment"># 5</span>
<span class="comment"># 6</span>
<span class="comment"># 7</span>
<span class="comment"># 8</span>
<span class="comment"># 9</span>

<span class="comment"># Note that the chr functions takes in a number</span>
<span class="comment"># and returns the ascii character for the number</span>
capital_letters = []
<span class="keyword">for</span> num <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">65</span>,<span class="integer">91</span>):
    capital_letters.append(<span class="predefined">chr</span>(num))

capital_letters
<span class="comment"># Output:['A','B','C','D','E','F','G','H','I','J',</span>
<span class="comment">#   'K','L','M','N','O','P','Q','R',</span>
<span class="comment">#   'S','T','U','V','W','X','Y','Z']</span>
</pre></div>
</div>

<p>Ranges take up less memory than lists, so if you find yourself needing a bunch of numbers that increment by the same amount each time, try to use a range instead of a list.</p>

<h3>List Comprehension</h3>

<p>List comprehensions are one of the most powerful tools in Python. They allow you to build lists in a more concise way, often in a single line. List comprehensions are a wonderful alternative to loops!</p>

<p>One way to use a list comprehension is to transform a set of values from a range or another list into some new set of values. This is sometimes referred to as a mapping opration. Here are a few examples:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># return a list of squares</span>
[num**<span class="integer">2</span> <span class="keyword">for</span> num <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">10</span>)] <span class="comment"># [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]</span>

[<span class="predefined">chr</span>(num) <span class="keyword">for</span> num <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">65</span>,<span class="integer">91</span>)]
<span class="comment"># Output:['A','B','C','D','E','F','G','H','I','J',</span>
<span class="comment">#   'K','L','M','N','O','P','Q','R',</span>
<span class="comment">#   'S','T','U','V','W','X','Y', 'Z']</span>
</pre></div>
</div>

<p>We can also put <code>if</code> statements inside of our list comprehensions to filter out certain transformed values!</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># option 1 without list comprehension</span>
vowels = []
<span class="keyword">for</span> letter <span class="keyword">in</span> <span class="string"><span class="delimiter">'</span><span class="content">awesome</span><span class="delimiter">'</span></span>:
    <span class="keyword">if</span> letter <span class="keyword">in</span> [<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">i</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">o</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">u</span><span class="delimiter">'</span></span>]:
        vowels.append(letter)

print(vowels) <span class="comment"># ['a', 'e', 'o', 'e']</span>

<span class="comment"># option 2 with list comprehension</span>
<span class="comment"># In this example, the first letter is the value that we want in the new list</span>
<span class="comment"># and the if portion is the filter step</span>
vowels = [letter <span class="keyword">for</span> letter <span class="keyword">in</span> <span class="string"><span class="delimiter">'</span><span class="content">awesome</span><span class="delimiter">'</span></span> <span class="keyword">if</span> letter <span class="keyword">in</span> [<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">i</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">o</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">u</span><span class="delimiter">'</span></span>]]
print(vowels) <span class="comment"># ['a', 'e', 'o', 'e']</span>

<span class="comment"># Count of 3 letter words in a string</span>
<span class="predefined">len</span>([word <span class="keyword">for</span> word <span class="keyword">in</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">the quick brown fox jumps over the lazy dog</span><span class="delimiter">&quot;</span></span>.split(<span class="string"><span class="delimiter">&quot;</span><span class="content"> </span><span class="delimiter">&quot;</span></span>) <span class="keyword">if</span> <span class="predefined">len</span>(word) == <span class="integer">3</span>])

<span class="comment"># figure out the length</span>
    <span class="comment"># for each word in the string &quot;the quick brown fox jumps over the lazy dog&quot; split(&quot; &quot;) into an array</span>
        <span class="comment"># if the length of each word is 3</span>
</pre></div>
</div>

<p>For longer list comprehensions, we can also split it into multiple lines for readability:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="predefined">len</span>([
    word
    <span class="keyword">for</span> word <span class="keyword">in</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">the quick brown fox jumps over the lazy dog</span><span class="delimiter">&quot;</span></span>.split(<span class="string"><span class="delimiter">&quot;</span><span class="content"> </span><span class="delimiter">&quot;</span></span>)
    <span class="keyword">if</span> <span class="predefined">len</span>(word) == <span class="integer">3</span>
])
</pre></div>
</div>

<p>The syntax for list comprehension takes some getting used to, but keep practicing and you will start to find it very useful.</p>


When you're ready, move on to List Exercises

<h1> List Exercises</h1>

<h3>Part I</h3>

<p>Write the following Python code to do the following (complete ALL of these using list comprehension).</p>

<ol>
<li>Given a list <code>[1,2,3,4]</code>, print out all the values in the list.</li>
<li>Given a list <code>[1,2,3,4]</code>, print out all the values in the list multiplied by 20.</li>
<li>Given a list <code>[&quot;Elie&quot;, &quot;Tim&quot;, &quot;Matt&quot;]</code>, return a new list with only the first letter (<code>[&quot;E&quot;, &quot;T&quot;, &quot;M&quot;]</code>).</li>
<li>Given a list <code>[1,2,3,4,5,6]</code> return a new list of all the even values (<code>[2,4,6]</code>).</li>
<li>Given two lists <code>[1,2,3,4]</code> and <code>[3,4,5,6]</code>, return a new list that is the intersection of the two (<code>[3,4]</code>).</li>
<li>Given a list of words <code>[&quot;Elie&quot;, &quot;Tim&quot;, &quot;Matt&quot;]</code> return a new list with each word reversed and in lower case (<code>[&#39;eile&#39;, &#39;mit&#39;, &#39;ttam&#39;]</code>).</li>
<li>Given two strings &quot;first&quot; and &quot;third&quot;, return a new string with all the letters present in both words (<code>[&quot;i&quot;, &quot;r&quot;, &quot;t&quot;]</code>).</li>
<li>For all the numbers between 1 and 100, return a list with all the numbers that are divisible by 12 (<code>[12, 24, 36, 48, 60, 72, 84, 96]</code>).</li>
<li>Given the string &quot;amazing&quot;, return a list with all the vowels removed (<code>[&#39;m&#39;, &#39;z&#39;, &#39;n&#39;, &#39;g&#39;]</code>).</li>
<li>Generate a list with the value <code>[[0, 1, 2], [0, 1, 2], [0, 1, 2]]</code>.</li>
<li><p>Generate a list with the value: </p>
<div class="CodeRay">
  <div class="code"><pre>[
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>],
 [<span class="integer">0</span>, <span class="integer">1</span>, <span class="integer">2</span>, <span class="integer">3</span>, <span class="integer">4</span>, <span class="integer">5</span>, <span class="integer">6</span>, <span class="integer">7</span>, <span class="integer">8</span>, <span class="integer">9</span>]
]
</pre></div>
</div></li>
</ol>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_1_solutions/blob/master/python_lists/solutions.md">here</a>.</p>

When you're ready, move on to Dictionary Basics

<h1> Dictionary Basics</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Create a Python dictionary</li>
<li>Access values in an dictionary</li>
<li>Modify the values stored in a dictionary</li>
<li>Determine if a key exists in a dictionary </li>
<li>Use common dictionary methods</li>
</ul>

<h3>Dictionaries</h3>

<p>Dictionaries in Python are key-value pairs. To access a value in a dictionary, you pass the key in using square brackets.</p>

<p>There are a few different ways to create a dictionary. One is to use curly braces, separating key-value pairs by a comma, and placing a colon between the key and the value:</p>
<div class="CodeRay">
  <div class="code"><pre>authors = {
    <span class="string"><span class="delimiter">'</span><span class="content">Great Gatsby</span><span class="delimiter">'</span></span>: <span class="string"><span class="delimiter">'</span><span class="content">F Scott Fitzgerald</span><span class="delimiter">'</span></span>,
    <span class="string"><span class="delimiter">'</span><span class="content">Slaughterhouse Five</span><span class="delimiter">'</span></span>: <span class="string"><span class="delimiter">'</span><span class="content">Kurt Vonnegut</span><span class="delimiter">'</span></span>,
    <span class="string"><span class="delimiter">'</span><span class="content">Of Mice and Men</span><span class="delimiter">'</span></span>: <span class="string"><span class="delimiter">'</span><span class="content">John Steinbeck</span><span class="delimiter">'</span></span>
}

authors[<span class="string"><span class="delimiter">'</span><span class="content">Great Gatsby</span><span class="delimiter">'</span></span>] == <span class="string"><span class="delimiter">'</span><span class="content">F Scott Fitzgerald</span><span class="delimiter">'</span></span> <span class="comment"># True</span>
</pre></div>
</div>

<p>Another approach is to use the <code>dict</code> function. In this case, you can assign values to keys directly using <code>=</code>:</p>
<div class="CodeRay">
  <div class="code"><pre>another_dictionary = <span class="predefined">dict</span>(key = <span class="string"><span class="delimiter">'</span><span class="content">value</span><span class="delimiter">'</span></span>)
another_dictionary <span class="comment"># {'key': 'value'}</span>
another_dictionary[<span class="string"><span class="delimiter">'</span><span class="content">key</span><span class="delimiter">'</span></span>] == <span class="string"><span class="delimiter">'</span><span class="content">value</span><span class="delimiter">'</span></span> <span class="comment"># True</span>
another_dictionary[<span class="string"><span class="delimiter">'</span><span class="content">another_key</span><span class="delimiter">'</span></span>] <span class="comment"># KeyError</span>
</pre></div>
</div>

<p>Note that if you try to access a value with a key that doesn&#39;t exist in the dictionary, Python will throw an error.</p>

<p>As with lists, we can reassign values to existing keys by using <code>=</code>. We can also use this to create new key-value pairs:</p>
<div class="CodeRay">
  <div class="code"><pre>another_dictionary = <span class="predefined">dict</span>(key = <span class="string"><span class="delimiter">'</span><span class="content">value</span><span class="delimiter">'</span></span>)
another_dictionary[<span class="string"><span class="delimiter">'</span><span class="content">key</span><span class="delimiter">'</span></span>] = <span class="string"><span class="delimiter">'</span><span class="content">new value</span><span class="delimiter">'</span></span>
another_dictionary[<span class="string"><span class="delimiter">'</span><span class="content">another_key</span><span class="delimiter">'</span></span>] = <span class="string"><span class="delimiter">'</span><span class="content">another value</span><span class="delimiter">'</span></span>
another_dictionary <span class="comment"># {'another_key': 'another value', 'key': 'new value'}</span>
</pre></div>
</div>

<p>Here are some common methods on dictionaries (in alphabetical order):</p>

<h4><code>clear</code></h4>

<p>Clears all the keys and values in a dictionary:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
d.clear()
d <span class="comment"># {}</span>
</pre></div>
</div>

<h4><code>copy</code></h4>

<p>Makes a copy of a dictionary:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
c = d.copy()
c <span class="comment"># {'a': 1, 'b': 2, 'c': 3}</span>
c <span class="keyword">is</span> d <span class="comment"># False - this really is a copy, not the original dictionary</span>
</pre></div>
</div>

<h4><code>fromkeys</code></h4>

<p>Creates key-value pairs from comma separated values:</p>
<div class="CodeRay">
  <div class="code"><pre>{}.fromkeys(<span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>,<span class="string"><span class="delimiter">&quot;</span><span class="content">b</span><span class="delimiter">&quot;</span></span>) <span class="comment"># {'a': 'b'}</span>
{}.fromkeys(<span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>,[<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>]) <span class="comment"># {'a': [1, 2, 3, 4, 5]}</span>
</pre></div>
</div>

<h4><code>get</code></h4>

<p>Retrieves a key in an object and return <code>None</code> instead of a <code>KeyError</code> if the key does not exist:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
d[<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>] <span class="comment"># 1</span>
d.get(<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>) <span class="comment"># 1</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">b</span><span class="delimiter">'</span></span>] <span class="comment"># 2</span>
d.get(<span class="string"><span class="delimiter">'</span><span class="content">b</span><span class="delimiter">'</span></span>) <span class="comment"># 2</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">no_key</span><span class="delimiter">'</span></span>] <span class="comment"># KeyError</span>
d.get(<span class="string"><span class="delimiter">'</span><span class="content">no_key</span><span class="delimiter">'</span></span>) <span class="comment"># None</span>
</pre></div>
</div>

<h4><code>items</code></h4>

<p>Returns a list of tuples with each key-value pair:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
d.items() <span class="comment"># dict_items([('a', 1), ('b', 2), ('c', 3)])</span>
</pre></div>
</div>

<h4><code>keys</code></h4>

<p>Returns a <code>dict_keys</code> object containing all of the keys in an object.</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
d.keys() <span class="comment"># dict_keys(['a', 'b', 'c'])</span>
</pre></div>
</div>

<h4><code>pop</code></h4>

<p>Takes a single argument corresponding to a key and removes that key-value pair from the dictionary. Returns the value corresponding to the key that was removed. Unlike <code>pop</code> on lists, you <em>must</em> supply an argument to the dictionary pop method or you&#39;ll get an error. You&#39;ll also get an error if you try to pop a key that doesn&#39;t exist in the dictionary.</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>)
d.pop() <span class="comment"># TypeError: pop expected at least 1 arguments, got 0</span>
d.pop(<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>) <span class="comment"># 1</span>
d <span class="comment"># {'c': 3, 'b': 2}</span>
d.pop(<span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>) <span class="comment"># KeyError</span>
</pre></div>
</div>

<h4><code>popitem</code></h4>

<p>Removes a random key in a dictionary:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>,d=<span class="integer">4</span>,e=<span class="integer">5</span>)
d.popitem() <span class="comment"># ('d', 4)</span>
d.popitem(<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>) <span class="comment"># TypeError: popitem() takes no arguments (1 given)</span>
</pre></div>
</div>

<h4><code>update</code></h4>

<p>Update keys and values in a dictionary with another set of key value pairs.</p>
<div class="CodeRay">
  <div class="code"><pre>first = <span class="predefined">dict</span>(a=<span class="integer">1</span>,b=<span class="integer">2</span>,c=<span class="integer">3</span>,d=<span class="integer">4</span>,e=<span class="integer">5</span>)
second = {}

second.update(first)
second <span class="comment"># {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}</span>

<span class="comment"># let's overwrite an existng key</span>
second[<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>] = <span class="string"><span class="delimiter">&quot;</span><span class="content">AMAZING</span><span class="delimiter">&quot;</span></span>

<span class="comment"># if we update again</span>
second.update(first) <span class="comment"># {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}</span>

<span class="comment"># the update overrides our values</span>
second <span class="comment"># {'a': 1, 'b': 2, 'c': 3, 'd': 4, 'e': 5}</span>
</pre></div>
</div>

When you're ready, move on to Dictionary Iteration and Comprehension


<h1>Dictionary Iteration and Comprehension.</h1>
 
 <h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Understand how to iterate through a dictionary </li>
<li>Create dictionaries using dictionary comprehension</li>
<li>Understand how to use data structures like <code>tuples</code> and <code>sets</code></li>
</ul>

<h3>Dictionary iteration</h3>

<p>As with lists, we can use a <code>for in</code> loop to iterate through a dictionary. By default, the loop will iterate through the keys:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(name = <span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>, job = <span class="string"><span class="delimiter">'</span><span class="content">Instructor</span><span class="delimiter">'</span></span>)

<span class="keyword">for</span> k <span class="keyword">in</span> d:
    print(k)

<span class="comment"># name</span>
<span class="comment"># job</span>
</pre></div>
</div>

<p>If you want access to both the keys and the values, call <code>items</code> on the dictionary and iterate through the result:</p>
<div class="CodeRay">
  <div class="code"><pre>d = <span class="predefined">dict</span>(name = <span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>, job = <span class="string"><span class="delimiter">'</span><span class="content">Instructor</span><span class="delimiter">'</span></span>)

<span class="keyword">for</span> key, value <span class="keyword">in</span> d.items():
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">{}:{}</span><span class="delimiter">&quot;</span></span>.format(key,value))

<span class="comment"># name:Elie</span>
<span class="comment"># job:Instructor</span>
</pre></div>
</div>

<h3>Dictionary comprehension</h3>

<p>We can convert dictionaries into lists using list comprehension:</p>
<div class="CodeRay">
  <div class="code"><pre>d = {<span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>: <span class="integer">1</span>, <span class="string"><span class="delimiter">'</span><span class="content">c</span><span class="delimiter">'</span></span>: <span class="integer">3</span>, <span class="string"><span class="delimiter">'</span><span class="content">e</span><span class="delimiter">'</span></span>: <span class="integer">5</span>}
[v <span class="keyword">for</span> k,v <span class="keyword">in</span> d.items()] <span class="comment"># [1, 5, 3]</span>
[k <span class="keyword">for</span> k,v <span class="keyword">in</span> d.items()] <span class="comment"># ['a', 'e', 'c']</span>
</pre></div>
</div>

<p>But we can also convert other data types into dictionaries using dictionary comprehension!</p>
<div class="CodeRay">
  <div class="code"><pre>str1 = <span class="string"><span class="delimiter">&quot;</span><span class="content">ABC</span><span class="delimiter">&quot;</span></span>
str2 = <span class="string"><span class="delimiter">&quot;</span><span class="content">123</span><span class="delimiter">&quot;</span></span>
{str1[i]: str2[i] <span class="keyword">for</span> i <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">0</span>,<span class="predefined">len</span>(str1))} <span class="comment"># {'A': '1', 'B': '2', 'C': '3'}</span>
</pre></div>
</div>

<p>Whoaaa, what did we just do? Let&#39;s take a step back. We took each string at the character <code>i</code>, where <code>i</code> ranges over all whole numbers from 0 to 2. At each step, we&#39;re setting the character at index <code>i</code> in <code>str1</code> and setting it as a new key, with a value coming from the same index in <code>str2</code>. </p>

<p>Let&#39;s look at another dictionary comprehension example. This time, we&#39;ll take a list of numbers <code>[1,2,3,4]</code> and return a dictionary with the key as the number and the value as &quot;odd&quot; or &quot;even&quot;. We can do some pretty cool stuff with dictionary comprehension here. Take a look!</p>
<div class="CodeRay">
  <div class="code"><pre>num_list = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]
{ num:(<span class="string"><span class="delimiter">&quot;</span><span class="content">even</span><span class="delimiter">&quot;</span></span> <span class="keyword">if</span> num % <span class="integer">2</span> == <span class="integer">0</span> <span class="keyword">else</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">odd</span><span class="delimiter">&quot;</span></span>) <span class="keyword">for</span> num <span class="keyword">in</span> num_list }
</pre></div>
</div>

<h3>Tuples</h3>

<p>Tuples are another collection in Python, but they are <em>immutable</em>. This means that you can&#39;t reassign values in tuples like you can with lists. Because of this immutability, however, operations on tuples are faster than lists. If you&#39;re defining a collection of values that won&#39;t change (for instance, maybe all you&#39;re ever going to do with it is iterate through it), use a tuple instead of a list.</p>
<div class="CodeRay">
  <div class="code"><pre>x = (<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>)
<span class="integer">3</span> <span class="keyword">in</span> x <span class="comment"># True</span>
x[<span class="integer">0</span>] = <span class="string"><span class="delimiter">&quot;</span><span class="content">change me!</span><span class="delimiter">&quot;</span></span> <span class="comment"># TypeError: 'tuple' object does not support item assignment</span>
</pre></div>
</div>

<p>Here are some common methods used on tuples (in alphabetical order):</p>

<h4><code>count</code></h4>

<p>Returns the number of times a value appears in a tuple:</p>
<div class="CodeRay">
  <div class="code"><pre>x = (<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">3</span>,<span class="integer">3</span>)
x.count(<span class="integer">1</span>) <span class="comment"># 1</span>
x.count(<span class="integer">3</span>) <span class="comment"># 3</span>
</pre></div>
</div>

<h4><code>index</code></h4>

<p>Returns the index at which a value is found in a tuple.</p>
<div class="CodeRay">
  <div class="code"><pre>t = (<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">3</span>,<span class="integer">3</span>)
t.index(<span class="integer">1</span>) <span class="comment"># 0</span>
t.index(<span class="integer">5</span>) <span class="comment"># ValueError: tuple.index(x): x not in tuple</span>
t.index(<span class="integer">3</span>) <span class="comment"># 2 - only the first matching index is returned</span>
</pre></div>
</div>

<h3>Sets</h3>

<p>Sets do not have duplicate values, and elements in sets aren&#39;t ordered.  You cannot access items in a set by index. Sets can be useful if you need to keep track of a collection of elements, but don&#39;t care about ordering. For example, if you wanted to check whether a certain number is prime, it would be helpful if you had a set of prime numbers to check against.</p>

<p>To test whether a value is a member of a set, use the <code>in</code> operator:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># Sets cannot have duplictes</span>
s = <span class="predefined">set</span>({<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">5</span>,<span class="integer">5</span>}) <span class="comment"># {1, 2, 3, 4, 5}</span>

<span class="comment"># Creating a new set</span>
s = <span class="predefined">set</span>({<span class="integer">1</span>,<span class="integer">4</span>,<span class="integer">5</span>})

<span class="comment"># Creates a set with the same values as above</span>
s = {<span class="integer">4</span>,<span class="integer">1</span>,<span class="integer">5</span>}

<span class="comment"># True</span>
<span class="integer">4</span> <span class="keyword">in</span> s

<span class="comment"># False</span>
<span class="integer">8</span> <span class="keyword">in</span> s
</pre></div>
</div>

<p>Here are some set methods (in alphabetical order):</p>

<h4><code>add</code></h4>

<p>Adds an element to a set. If the element is already in the set, the set doesn&#39;t change:</p>
<div class="CodeRay">
  <div class="code"><pre>s = <span class="predefined">set</span>([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>])
s.add(<span class="integer">4</span>)
s <span class="comment"># {1, 2, 3, 4}</span>
s.add(<span class="integer">4</span>)
s <span class="comment"># {1, 2, 3, 4}</span>
</pre></div>
</div>

<h4><code>clear</code></h4>

<p>Removes all the contents of the set:</p>
<div class="CodeRay">
  <div class="code"><pre>s = <span class="predefined">set</span>([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>])
s.clear()
s <span class="comment"># set()</span>
</pre></div>
</div>

<h4><code>copy</code></h4>

<p>Creates a copy of the set:</p>
<div class="CodeRay">
  <div class="code"><pre>s = <span class="predefined">set</span>([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>])
another_s = s.copy()
another_s <span class="comment"># {1, 2, 3}</span>
another_s <span class="keyword">is</span> s <span class="comment"># False</span>
</pre></div>
</div>

<h4><code>difference</code></h4>

<p>Returns a new set containing all the elements that are in the first set but not in the set passed to <code>difference</code>:</p>
<div class="CodeRay">
  <div class="code"><pre>set1 = {<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>}
set2 = {<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>}
set1.difference(set2) <span class="comment"># {1}</span>
set2.difference(set1) <span class="comment"># {4}</span>
</pre></div>
</div>

<h4><code>intersection</code></h4>

<p>Returns a new set containing all the elements that are in both sets:</p>
<div class="CodeRay">
  <div class="code"><pre>set1 = {<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>}
set2 = {<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>}
set1.intersection(set2) <span class="comment"># {2,3}</span>
</pre></div>
</div>

<h4><code>symmetric_difference</code></h4>

<p>Returns a new set containing all the elements that are in exactly one of the sets:</p>
<div class="CodeRay">
  <div class="code"><pre>set1 = {<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>}
set2 = {<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>}
set1.symmetric_difference(set2) <span class="comment"># {1,4}</span>
</pre></div>
</div>

<h4><code>union</code></h4>

<p>Returns a new set containing all the elements that are in either set:</p>
<div class="CodeRay">
  <div class="code"><pre>set1 = {<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>}
set2 = {<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>}
set1.union(set2) <span class="comment"># {1,2,3,4}</span>
</pre></div>
</div>

When you're ready, move on to Dictionary Exercises

<h1> Dictionary Exercises. </h1>


<p>Write the following Python code to do the following (Complete ALL of the following using <code>dictionary comprehension</code>)</p>

<ol>
<li>Given a list <code>[(&quot;name&quot;, &quot;Elie&quot;), (&quot;job&quot;, &quot;Instructor&quot;)]</code>, create a dictionary that looks like this <code>{&#39;job&#39;: &#39;Instructor&#39;, &#39;name&#39;: &#39;Elie&#39;}</code> (the order does not matter).</li>
<li>Given two lists <code>[&quot;CA&quot;, &quot;NJ&quot;, &quot;RI&quot;]</code> and <code>[&quot;California&quot;, &quot;New Jersey&quot;, &quot;Rhode Island&quot;]</code> return a dictionary that looks like this <code>{&#39;CA&#39;: &#39;California&#39;, &#39;NJ&#39;: &#39;New Jersey&#39;, &#39;RI&#39;: &#39;Rhode Island&#39;}</code>. You can research the <code>zip</code> method to help you.</li>
<li>Create a dictionary with the key as a vowel in the alphabet and the value as 0. Your dictionary should look like this <code>{&#39;a&#39;: 0, &#39;e&#39;: 0, &#39;i&#39;: 0, &#39;o&#39;: 0, &#39;u&#39;: 0}</code>. (Do not use the <code>fromkeys</code> method).</li>
<li>Create a dictionary starting with the key of the position of the letter and the value as the letter in the alphabet. You should return something like this (Hint - use <code>chr(65)</code> to get the first letter):</li>
</ol>
<div class="CodeRay">
  <div class="code"><pre>{<span class="integer">1</span>: <span class="string"><span class="delimiter">'</span><span class="content">A</span><span class="delimiter">'</span></span>,
 <span class="integer">2</span>: <span class="string"><span class="delimiter">'</span><span class="content">B</span><span class="delimiter">'</span></span>,
 <span class="integer">3</span>: <span class="string"><span class="delimiter">'</span><span class="content">C</span><span class="delimiter">'</span></span>,
 <span class="integer">4</span>: <span class="string"><span class="delimiter">'</span><span class="content">D</span><span class="delimiter">'</span></span>,
 <span class="integer">5</span>: <span class="string"><span class="delimiter">'</span><span class="content">E</span><span class="delimiter">'</span></span>,
 <span class="integer">6</span>: <span class="string"><span class="delimiter">'</span><span class="content">F</span><span class="delimiter">'</span></span>,
 <span class="integer">7</span>: <span class="string"><span class="delimiter">'</span><span class="content">G</span><span class="delimiter">'</span></span>,
 <span class="integer">8</span>: <span class="string"><span class="delimiter">'</span><span class="content">H</span><span class="delimiter">'</span></span>,
 <span class="integer">9</span>: <span class="string"><span class="delimiter">'</span><span class="content">I</span><span class="delimiter">'</span></span>,
 <span class="integer">10</span>: <span class="string"><span class="delimiter">'</span><span class="content">J</span><span class="delimiter">'</span></span>,
 <span class="integer">11</span>: <span class="string"><span class="delimiter">'</span><span class="content">K</span><span class="delimiter">'</span></span>,
 <span class="integer">12</span>: <span class="string"><span class="delimiter">'</span><span class="content">L</span><span class="delimiter">'</span></span>,
 <span class="integer">13</span>: <span class="string"><span class="delimiter">'</span><span class="content">M</span><span class="delimiter">'</span></span>,
 <span class="integer">14</span>: <span class="string"><span class="delimiter">'</span><span class="content">N</span><span class="delimiter">'</span></span>,
 <span class="integer">15</span>: <span class="string"><span class="delimiter">'</span><span class="content">O</span><span class="delimiter">'</span></span>,
 <span class="integer">16</span>: <span class="string"><span class="delimiter">'</span><span class="content">P</span><span class="delimiter">'</span></span>,
 <span class="integer">17</span>: <span class="string"><span class="delimiter">'</span><span class="content">Q</span><span class="delimiter">'</span></span>,
 <span class="integer">18</span>: <span class="string"><span class="delimiter">'</span><span class="content">R</span><span class="delimiter">'</span></span>,
 <span class="integer">19</span>: <span class="string"><span class="delimiter">'</span><span class="content">S</span><span class="delimiter">'</span></span>,
 <span class="integer">20</span>: <span class="string"><span class="delimiter">'</span><span class="content">T</span><span class="delimiter">'</span></span>,
 <span class="integer">21</span>: <span class="string"><span class="delimiter">'</span><span class="content">U</span><span class="delimiter">'</span></span>,
 <span class="integer">22</span>: <span class="string"><span class="delimiter">'</span><span class="content">V</span><span class="delimiter">'</span></span>,
 <span class="integer">23</span>: <span class="string"><span class="delimiter">'</span><span class="content">W</span><span class="delimiter">'</span></span>,
 <span class="integer">24</span>: <span class="string"><span class="delimiter">'</span><span class="content">X</span><span class="delimiter">'</span></span>,
 <span class="integer">25</span>: <span class="string"><span class="delimiter">'</span><span class="content">Y</span><span class="delimiter">'</span></span>,
 <span class="integer">26</span>: <span class="string"><span class="delimiter">'</span><span class="content">Z</span><span class="delimiter">'</span></span>}
</pre></div>
</div>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_1_solutions/blob/master/python_dictionaries/solutions.md">here</a>.</p>

When you're ready, move on to Functions Basics 

<h1> Functions Basics. </h1>

<h3>Functions</h3>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Explain the value and purpose of a function</li>
<li>Understand how to return output from functions</li>
</ul>

<h3>What is a function?</h3>

<p>A function is a repeatable process or procedure.  A real world analogy of a function is the brew button on a coffee machine.  The coffee machine has inputs (hot water, coffee grounds), and outputs (hot coffee).  When you press the button to brew a pot of coffee, you are starting a process that should return an expected output to you.  The same thing is true in programming.  A function takes a set of variables as inputs and returns a value as an output.</p>

<p>We have already seen many functions in action.  For example, in the list chapter, we learned about <code>append</code> and many others.  These are built-in functions that operate on a list. But in addition to built in-functions, we can also write our own functions! In Python, a function has the following format:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">function_name</span>():
    <span class="comment"># code gets indented here</span>
</pre></div>
</div>

<p>Notice that we <strong>MUST</strong> indent on the following line. If you do not indent your code, you&#39;ll get an <code>IndentationError</code>! To invoke a function, use the <code>()</code>:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">first_function</span>():
  print(<span class="string"><span class="delimiter">&quot;</span><span class="content">Hello World!</span><span class="delimiter">&quot;</span></span>)

first_function() <span class="comment"># Hello World!</span>
</pre></div>
</div>

<p>Next, let&#39;s try to write a function called <code>add_five_plus_five</code> which outputs the sum of 5 + 5. Here&#39;s what that might look like:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add_five_plus_five</span>():
    <span class="integer">5</span>+<span class="integer">5</span>
</pre></div>
</div>

<p>Now let&#39;s run this function <code>add_five_plus_five()</code> and our output is....nothing! Why is that? We are missing a very important keyword: <code>return</code>.</p>

<p>In order to output values from a function, we need to use the <code>return</code> keyword. Let&#39;s see how we can fix our function now. </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add_five_plus_five</span>():
    <span class="keyword">return</span> <span class="integer">5</span>+<span class="integer">5</span>
</pre></div>
</div>

<p>Now let&#39;s run this function <code>add_five_plus_five()</code> and our output is....10! If we would like, we can also save this information to a variable and use it at a later point in time like this:</p>
<div class="CodeRay">
  <div class="code"><pre>ten = add_five_plus_five()
print(ten + <span class="integer">10</span>) <span class="comment"># 20</span>
</pre></div>
</div>

<p>If we don&#39;t have a return statement in our function, it will always return <code>None</code> to us. This is true regardless of what else happens in the function. Take a look at this example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">print_five_plus_five</span>():
    print(<span class="integer">5</span> + <span class="integer">5</span>)

<span class="keyword">def</span> <span class="function">add_five_plus_five</span>():
    <span class="keyword">return</span> <span class="integer">5</span> + <span class="integer">5</span>

ten = add_five_plus_five()
maybe_ten = print_five_plus_five() <span class="comment"># this line should print 10 to the console</span>

ten <span class="comment"># 10</span>
maybe_ten <span class="comment"># None</span>
</pre></div>
</div>

<p>In the real world, we&#39;d never really write functions like these because they are very rigid; all they do is add 5 and 5. Ideally, we&#39;d like to be able to provide some input to our functions, but in order to do that we need to introduce a concept called <code>parameters</code> or <code>arguments</code>.</p>

When you're ready, move on to Function Parameters

<h1>Function Parameters </h1>

 <h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Define what a parameter is and why they are essential when writing functions</li>
<li>Understand what keyword arguments are </li>
<li>Use default arguments in python functions</li>
<li>Define functions that accept an unknown number of arguments</li>
</ul>

<h3>Functions with arguments</h3>

<p>Here is an example of a function that takes two arguments:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">pet_names</span>(cat_name, dog_name):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">I have a cat named {} and a dog named {}.</span><span class="delimiter">&quot;</span></span>.format(cat_name, dog_name)
</pre></div>
</div>

<p>In this case, our function takes two arguments (a <code>cat_name</code> and a <code>dog_name</code>), and <code>return</code>s a message about the pets.</p>

<h3>Keyword arguments</h3>

<p>One nice thing about Python is that if you know the names of the arguments that you will pass to a function, you can pass them into the function in any order. All you need to do is provide the name (or keyword) for the argument, then the value you want to pass in. Check it out:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">pet_names</span>(cat_name, dog_name):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">I have a cat named {} and a dog named {}.</span><span class="delimiter">&quot;</span></span>.format(cat_name, dog_name)

<span class="comment"># no keyword arguments - order matters!</span>
pet_names(<span class="string"><span class="delimiter">&quot;</span><span class="content">Mittens</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">Fido</span><span class="delimiter">&quot;</span></span>) <span class="comment"># &quot;I have a cat named Mittens and a dog named Fido.&quot;</span>

pet_names(<span class="string"><span class="delimiter">&quot;</span><span class="content">Fido</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">Mittens</span><span class="delimiter">&quot;</span></span>) <span class="comment"># &quot;I have a cat named Fido and a dog named Mittens.&quot; -- uh oh, the names are the opposite of what we want, because we passed them to the function in the wrong order.</span>

<span class="comment"># keyword arguments</span>
pet_names(cat_name=<span class="string"><span class="delimiter">&quot;</span><span class="content">Mittens</span><span class="delimiter">&quot;</span></span>, dog_name=<span class="string"><span class="delimiter">&quot;</span><span class="content">Fido</span><span class="delimiter">&quot;</span></span>)
<span class="comment"># &quot;I have a cat named Mittens and a dog named Fido.&quot;</span>

<span class="comment"># keyword arguments - order doesn't matter!</span>
pet_names(dog_name=<span class="string"><span class="delimiter">&quot;</span><span class="content">Fido</span><span class="delimiter">&quot;</span></span>, cat_name=<span class="string"><span class="delimiter">&quot;</span><span class="content">Mittens</span><span class="delimiter">&quot;</span></span>)
<span class="comment"># &quot;I have a cat named Mittens and a dog named Fido.&quot;</span>
</pre></div>
</div>

<p>When you call a function by passing in a <code>keyword=value</code> pair, you&#39;re said to be using <em>keyword arguments</em>. This can be especially useful if you have a function that accepts many parameters.</p>

<h3>Default argument values</h3>

<p>Sometimes you may want to set default values for parameters you pass into your function. In Python, the syntax looks the same as when you use keyword arguments, with one crucial difference: you use keyword arguments when you <em>call</em> a function, but you use default argument values when you <em>define</em> a function. Here&#39;s an example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a=<span class="integer">5</span>,b=<span class="integer">15</span>):
    <span class="keyword">return</span> a + b
</pre></div>
</div>

<p>In this case, if we don&#39;t pass in any values when we call <code>add</code>, the first parameter will be 5 and the second parameter will be 15. But we can overwrite these defaults by simply passing numbers into the function when we call it:</p>
<div class="CodeRay">
  <div class="code"><pre>add(<span class="integer">15</span>,<span class="integer">1</span>) <span class="comment"># 16</span>
add(<span class="integer">4</span>) <span class="comment"># 19 - a is set to 4, b is set to 15</span>
add() <span class="comment"># 20</span>
add(b=<span class="integer">30</span>) <span class="comment"># 35 - a is set to 5 by default and b is 30 using keyword arguments</span>
</pre></div>
</div>

<h3>Variable number of function arguments</h3>

<p>Sometimes we might want to write a function that can be called with an unknown number of arguments. There are two ways we can do this. The first is by using <code>*</code>, in the function definition which allows us to pass in an unknown number of arguments:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">foo</span>(*args):
   print(args)

foo(<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>) <span class="comment"># (1,2,3)</span>
foo(<span class="integer">1</span>,<span class="integer">2</span>) <span class="comment"># (1,2)</span>
foo([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>]) <span class="comment"># ([1,2,3])</span>
</pre></div>
</div>

<p>Inside of the function, the named parameter after the <code>*</code> corresponds to a tuple of the arguments passed in.</p>

<p>This can be helpful if we want to iterate through all of the arguments or apply some other function on a tuple:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(*nums):
    <span class="keyword">return</span> <span class="predefined">sum</span>(nums)

add(<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>) <span class="comment"># 10</span>
</pre></div>
</div>

<p>We can also use the <code>*</code> operator when invoking a function. In that case, the <code>*</code> will take an iterable like a list and split it up into separate parameters.  Here is an example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add_three_nums</span>(n1, n2, n3):
    <span class="keyword">return</span> n1 + n2 + n3

add_three_nums(*[<span class="integer">5</span>,<span class="integer">6</span>,<span class="integer">4</span>]) <span class="comment"># same as add_three_nums(5,6,4)</span>
</pre></div>
</div>

<h3>Variable number of keyword arguments</h3>

<p>What if you want to pass in an unknown number of keyword arguments? In this case, we can use <code>**</code>, which allows us to access all of the keyword arguments inside of a function as a dictionary when we do not know how many keyword arguments will be passed.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">print_kwargs</span>(a,b,**kwargs):
    print(a,b,kwargs)

print_kwargs(<span class="integer">1</span>,<span class="integer">2</span>,awesome=<span class="string"><span class="delimiter">'</span><span class="content">sauce</span><span class="delimiter">'</span></span>, test=<span class="string"><span class="delimiter">'</span><span class="content">yup</span><span class="delimiter">'</span></span>) <span class="comment"># 1 2 {'test': 'yup', 'awesome': 'sauce'}</span>
</pre></div>
</div>

<p>You can read more about multiple function arguments <a target="_blank" href="http://agiliq.com/blog/2012/06/understanding-args-and-kwargs/">here</a>.</p>
When you're ready, move on to Function Scope

<h1> Function Scope</h1>
      <h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Define what scope is</li>
<li>Understand what globals and locals are</li>
<li>Document functions and specify data types for arguments and return values</li>
</ul>

<h3>Scope</h3>

<p>In Python we have function scope, which prohibits us from accessing variables created inside of a function from outside of that function:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">func</span>():
    x = <span class="integer">5</span>
    <span class="keyword">return</span> x

func() <span class="comment"># 5</span>
x <span class="comment"># NameError</span>
</pre></div>
</div>

<h3>The <code>global</code> keyword</h3>

<p>The global scope includes all variables defined outside of functions. But if we try to use a global variable in a method, we will see<br>
<code>UnboundLocalError: local variable VARIABLE_NAME referenced before assignment</code>.  This happens because a method in Python either has local variables or global variables.  If variable is defined <strong>anywhere</strong> in a method and that variable has the same name as a global variable, then the new local variable will be used in the function instead of the global.  But if you actually want to assign a global variable from within a function, you need to use the <code>global</code> keyword. Using global variables in general is <strong>not</strong> best practice:</p>
<div class="CodeRay">
  <div class="code"><pre>id = <span class="integer">0</span>
<span class="keyword">def</span> <span class="function">increment_id</span>():
    <span class="predefined">id</span> += <span class="integer">1</span>

increment_id() <span class="comment"># UnboundLocalError: local variable 'id' referenced before assignment</span>

<span class="keyword">def</span> <span class="function">increment_id</span>():
    <span class="keyword">global</span> <span class="predefined">id</span>
    <span class="predefined">id</span> += <span class="integer">1</span>

increment_id() <span class="comment"># The global id is now 1</span>
</pre></div>
</div>

<p>In Python you need to explicitly state that a variable should be global, using the <code>global</code> keyword.</p>

<h3>Listing locals and globals</h3>

<p>In Python we can display all of the local variables and global variables using the <code>locals</code> and <code>globals</code> functions</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">print_locals</span>():
    x = <span class="integer">2</span>
    name = <span class="string"><span class="delimiter">&quot;</span><span class="content">Elie</span><span class="delimiter">&quot;</span></span>
    print(<span class="predefined">locals</span>())

name = <span class="string"><span class="delimiter">&quot;</span><span class="content">person</span><span class="delimiter">&quot;</span></span>
print(<span class="predefined">globals</span>())
print(<span class="predefined">locals</span>())
</pre></div>
</div>

<h3>Python Nested Functions (sort of like closures)</h3>

<p>In Python we do have support for closures, a feature where an inner function has access to variables in an outer function&#39;s scope, even after the outer function has finished executing. </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">outer</span>(a):
    <span class="keyword">def</span> <span class="function">inner</span>(b):
        <span class="keyword">return</span> a + b
    <span class="keyword">return</span> inner

outer(<span class="integer">3</span>)(<span class="integer">4</span>) <span class="comment"># 7</span>
x = outer(<span class="integer">2</span>)
x(<span class="integer">10</span>) <span class="comment"># 12</span>
</pre></div>
</div>

<p>However, closures in Python are &quot;weak&quot; and have some limitations. For example, if you want to change the value of a variable from an outer scope, you&#39;ll run in to problems: </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">counter</span>():
    x = <span class="integer">0</span>;
    <span class="keyword">def</span> <span class="function">increment</span>():
        x += <span class="integer">1</span> 
        print(x)
    <span class="keyword">return</span> increment

counter()() <span class="comment"># UnboundLocalError: local variable 'x' referenced before assignment</span>
</pre></div>
</div>

<p>Again, this is because the <code>x</code> inside of <code>increment</code> is a new variable, bound to the scope of <code>increment</code>. It&#39;s not a reference to <code>x</code> coming from the scope of <code>counter</code>. </p>

<p>We can get around the problem with the example above by setting attributes on the inner function, rather than trying to change variables from an outer scope:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="comment"># We can get around this by doing</span>
<span class="keyword">def</span> <span class="function">outerCount</span>():
    <span class="keyword">def</span> <span class="function">innerCount</span>():
        innerCount.x += <span class="integer">1</span>
        print(innerCount.x)
    innerCount.x = <span class="integer">0</span>
    <span class="keyword">return</span> innerCount
</pre></div>
</div>

<p>You can read more about this concept of &quot;read only&quot; closures <a target="_blank" href="http://stackoverflow.com/questions/4020419/why-arent-python-nested-functions-called-closures">here</a>.</p>

<h3>Documenting our functions</h3>

<p>Something that Python offers us is the ability to add what is called a <code>docstring</code>. Let&#39;s see what that looks like</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">say_hello</span>():
    <span class="comment"># we are using three quotes so that this can be a multi-line string if necessary</span>
    <span class="docstring"><span class="delimiter">&quot;&quot;&quot;</span><span class="content">This function returns the string hello when called</span><span class="delimiter">&quot;&quot;&quot;</span></span>
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">hello</span><span class="delimiter">&quot;</span></span>
</pre></div>
</div>

<p>We can call this function using</p>
<div class="CodeRay">
  <div class="code"><pre>
say_hello() <span class="comment"># &quot;hello&quot;</span>

say_hello.__doc__ <span class="comment"># &quot;This function returns the string hello when called&quot;</span>

help(say_hello) <span class="comment"># gives us even more detail with the docstring!</span>
</pre></div>
</div>

<p>Docstrings are essential when writing methods and can be thought of like an enhanced comment. Docstrings are also very useful when writing tests, as you can see what the docstring is when running the test. You are <strong>highly</strong> encouraged to write docstrings for your functions, and inside classes as well. You can read more about standards on docstrings <a target="_blank" href="https://www.python.org/dev/peps/pep-0257/">here</a>.</p>

<h3>Default argument types for Python</h3>

<p>Unlike languages like Java and C++, Python is a loosely typed language. This means that we do not need to define the data type of a variable when initializing it. This gives us a bit more flexibility around our code, but sometimes we want to clearly indicate that a certain data type is what should be passed as a parameter, or that a function returns a specific value. We can do that in Python! Let&#39;s see what that looks like:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a: <span class="predefined">int</span>, b: <span class="predefined">int</span>) -&gt; <span class="predefined">int</span>:
    <span class="docstring"><span class="delimiter">&quot;&quot;&quot;</span><span class="content">This function returns the sum of two numbers</span><span class="delimiter">&quot;&quot;&quot;</span></span>
    <span class="keyword">return</span> a+b   
</pre></div>
</div>

<p>We are specifying that both <code>a</code> and <code>b</code> are <code>int</code>s and the return value from the function is an <code>int</code> as well. We can also combine this with default parameter values!</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a: int = <span class="integer">5</span> ,b: int = <span class="integer">5</span>) -&gt; <span class="predefined">int</span>:
    <span class="docstring"><span class="delimiter">&quot;&quot;&quot;</span><span class="content">This function returns the sum of two numbers with default values of 5 for a and 5 for b</span><span class="delimiter">&quot;&quot;&quot;</span></span>
    <span class="keyword">return</span> a+b
</pre></div>
</div>

When you're ready, move on to Functions Exercises

<h1>Functions Exercises</h1>
  <h3>Part I</h3>

<p>Write the following functions</p>

<h3><code>difference</code></h3>

<ul>
<li>this function takes in two parameters and returns the difference between the two</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>difference(<span class="integer">2</span>,<span class="integer">2</span>) <span class="comment"># 0</span>
difference(<span class="integer">0</span>,<span class="integer">2</span>) <span class="comment"># -2</span>
</pre></div>
</div>

<h3><code>product</code></h3>

<ul>
<li>this function takes in two parameters and returns the product of the two</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>product(<span class="integer">2</span>,<span class="integer">2</span>) <span class="comment"># 4</span>
product(<span class="integer">0</span>,<span class="integer">2</span>) <span class="comment"># 0</span>
</pre></div>
</div>

<h3><code>print_day</code></h3>

<ul>
<li>this function takes in one parameter (a number from 1-7) and returns the day of the week (1 is Sunday, 2 is Monday, 3 is Tuesday etc.). If the number is less than 1 or greater than 7, the function should return None</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>print_day(<span class="integer">4</span>) <span class="comment"># &quot;Wednesday&quot;</span>
print_day(<span class="integer">41</span>) <span class="comment"># None</span>
</pre></div>
</div>

<h3><code>last_element</code></h3>

<ul>
<li>this function takes in one parameter (a list) and returns the last value in the list. It should return None if the list is empty.</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>last_element([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]) <span class="comment"># 4</span>
last_element([]) <span class="comment"># None</span>
</pre></div>
</div>

<h3><code>number_compare</code></h3>

<ul>
<li>this function takes in two parameters (both numbers). If the first is greater than the second, this function returns &quot;First is greater.&quot; If the second number is greater than the first, the function returns &quot;Second is greater.&quot; Otherwise the function returns &quot;Numbers are equal.&quot;</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>number_compare(<span class="integer">1</span>,<span class="integer">1</span>) <span class="comment"># &quot;Numbers are equal&quot;</span>
number_compare(<span class="integer">1</span>,<span class="integer">2</span>) <span class="comment"># &quot;Second is greater&quot;</span>
number_compare(<span class="integer">2</span>,<span class="integer">1</span>) <span class="comment"># &quot;First is greater&quot;</span>
</pre></div>
</div>

<h3><code>single_letter_count</code></h3>

<ul>
<li>this function takes in two parameters (two strings). The first parameter should be a word and the second should be a letter. The function returns the number of times that letter appears in the word. The function should be case insensitive (does not matter if the input is lowercase or uppercase). If the letter is not found in the word, the function should return 0.</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>single_letter_count(<span class="string"><span class="delimiter">'</span><span class="content">amazing</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">A</span><span class="delimiter">'</span></span>) <span class="comment"># 2</span>
</pre></div>
</div>

<h3><code>multiple_letter_count</code></h3>

<ul>
<li>this function takes in one parameter (a string) and returns a dictionary with the keys being the letters and the values being the count of the letter.</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>multiple_letter_count(<span class="string"><span class="delimiter">&quot;</span><span class="content">hello</span><span class="delimiter">&quot;</span></span>) <span class="comment"># {h:1, e: 1, l: 2, o:1}</span>
multiple_letter_count(<span class="string"><span class="delimiter">&quot;</span><span class="content">person</span><span class="delimiter">&quot;</span></span>) <span class="comment"># {p:1, e: 1, r: 1, s:1, o:1, n:1}</span>
</pre></div>
</div>

<h3><code>list_manipulation</code></h3>

<ul>
<li>this function should take in three parameters (a list, command, location and value). 

<ul>
<li>If the command is &quot;remove&quot; and the location is &quot;end&quot;, the function should remove the last value in the list and return the value removed</li>
<li>If the command is &quot;remove&quot; and the location is &quot;beginning&quot;, the function should remove the first value in the list and return the value removed</li>
<li>If the command is &quot;add&quot; and the location is &quot;beginning&quot;, the function should add the value (fourth parameter) to the beginning of the list and return the list</li>
<li>If the command is &quot;add&quot; and the location is &quot;end&quot;, the function should add the value (fourth parameter) to the end of the list and return the list</li>
</ul></li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>list_manipulation([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>], <span class="string"><span class="delimiter">&quot;</span><span class="content">remove</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">end</span><span class="delimiter">&quot;</span></span>) <span class="comment"># 3</span>
list_manipulation([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>], <span class="string"><span class="delimiter">&quot;</span><span class="content">remove</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">beginning</span><span class="delimiter">&quot;</span></span>) <span class="comment"># 1</span>
list_manipulation([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>], <span class="string"><span class="delimiter">&quot;</span><span class="content">add</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">beginning</span><span class="delimiter">&quot;</span></span>, <span class="integer">20</span>) <span class="comment"># [20,1,2,3]</span>
list_manipulation([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>], <span class="string"><span class="delimiter">&quot;</span><span class="content">add</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">end</span><span class="delimiter">&quot;</span></span>, <span class="integer">30</span>) <span class="comment"># [1,2,3,30]</span>
</pre></div>
</div>

<h3><code>is_palindrome</code></h3>

<ul>
<li>A Palindrome is a word, phrase, number, or other sequence of characters which reads the same backward or forward. This function should take in one parameter and returns <code>True</code> or <code>False</code> depending on whether it is a palindrome. As a bonus, allow your function to ignore whitespace and capitalization so that <code>is_palindrome(&#39;a man a plan a canal Panama&#39;)</code> returns <code>True</code>.</li>
</ul>
<div class="CodeRay">
  <div class="code"><pre>is_palindrome(<span class="string"><span class="delimiter">'</span><span class="content">testing</span><span class="delimiter">'</span></span>) <span class="comment"># False</span>
is_palindrome(<span class="string"><span class="delimiter">'</span><span class="content">tacocat</span><span class="delimiter">'</span></span>) <span class="comment"># True</span>
is_palindrome(<span class="string"><span class="delimiter">'</span><span class="content">hannah</span><span class="delimiter">'</span></span>) <span class="comment"># True</span>
is_palindrome(<span class="string"><span class="delimiter">'</span><span class="content">robert</span><span class="delimiter">'</span></span>) <span class="comment"># False</span>
</pre></div>
</div>

<h3><code>frequency</code></h3>

<p>This function accepts a list and a <code>search_term</code> (this will always be a primitive value) and returns the number of times the <code>search_term</code> appears in the list.</p>
<div class="CodeRay">
  <div class="code"><pre>frequency([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">4</span>,<span class="integer">4</span>], <span class="integer">4</span>) <span class="comment"># 3</span>
frequency([<span class="predefined-constant">True</span>, <span class="predefined-constant">False</span>, <span class="predefined-constant">True</span>, <span class="predefined-constant">True</span>], <span class="predefined-constant">False</span>) <span class="comment"># 1</span>
</pre></div>
</div>

<h3><code>flip_case</code></h3>

<p>This function accepts a string and a letter and reverses the case of all occurances of the letter in the string.</p>
<div class="CodeRay">
  <div class="code"><pre>flip_case(<span class="string"><span class="delimiter">&quot;</span><span class="content">Hardy har har</span><span class="delimiter">&quot;</span></span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">h</span><span class="delimiter">&quot;</span></span>) <span class="comment"># &quot;hardy Har Har&quot;</span>
</pre></div>
</div>

<h3><code>multiply_even_numbers</code></h3>

<p>This function accepts a list of numbers and returns the product of all even numbers in the list.</p>
<div class="CodeRay">
  <div class="code"><pre>multiply_even_numbers([<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">6</span>]) <span class="comment"># 48</span>
</pre></div>
</div>

<h3><code>mode</code></h3>

<p>This function accepts a list of numbers and returns the most frequent number in the list of numbers. You can assume that the mode will be unique.</p>
<div class="CodeRay">
  <div class="code"><pre>mode([<span class="integer">2</span>,<span class="integer">4</span>,<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">4</span>,<span class="integer">4</span>,<span class="integer">6</span>,<span class="integer">4</span>,<span class="integer">6</span>,<span class="integer">7</span>,<span class="integer">4</span>]) <span class="comment"># 4</span>
</pre></div>
</div>

<h3><code>capitalize</code></h3>

<p>This function accepts a string and returns the same string with the first letter capitalized.</p>
<div class="CodeRay">
  <div class="code"><pre>capitalize(<span class="string"><span class="delimiter">&quot;</span><span class="content">tim</span><span class="delimiter">&quot;</span></span>) <span class="comment"># &quot;Tim&quot;</span>
capitalize(<span class="string"><span class="delimiter">&quot;</span><span class="content">matt</span><span class="delimiter">&quot;</span></span>) <span class="comment"># &quot;Matt&quot;</span>
</pre></div>
</div>

<h3><code>compact</code></h3>

<p>This function accepts a list and returns a list of values that are truthy values.</p>
<div class="CodeRay">
  <div class="code"><pre>compact([<span class="integer">0</span>,<span class="integer">1</span>,<span class="integer">2</span>,<span class="string"><span class="delimiter">&quot;</span><span class="delimiter">&quot;</span></span>,[], <span class="predefined-constant">False</span>, {}, <span class="predefined-constant">None</span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">All done</span><span class="delimiter">&quot;</span></span>]) <span class="comment"># [1,2, &quot;All done&quot;]</span>
</pre></div>
</div>

<h3><code>partition</code></h3>

<p>This function accepts a list and a callback function (which you can assume returns <code>True</code> or <code>False</code>). The function should iterate over each element in the list and invoke the callback function at each iteration. If the result of the callback function is <code>True</code>, the element should go into one list if it&#39;s <code>False</code>, the element should go into another list. When it&#39;s finished, <code>partition</code> should return both lists inside of one larger list.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">is_even</span>(num):
    <span class="keyword">return</span> num % <span class="integer">2</span> == <span class="integer">0</span>

partition([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>], is_even) <span class="comment"># [[2,4],[1,3]]</span>
</pre></div>
</div>

<h3><code>intersection</code></h3>

<p>This function should accept a two dimensional list and return a list with the values that are the same in each list.</p>
<div class="CodeRay">
  <div class="code"><pre>intersection([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>], [<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]) <span class="comment"># [2,3]</span>
</pre></div>
</div>

<h3><code>once</code></h3>

<p>This function accepts a function and returns a new function that can only be invoked once. If the function is invoked more than once, it should return <code>None</code>. <strong>Hint</strong> you will need to define a new function inside of your once function and return that function. You can add properties to your inner function to see if it has run already.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a+b

one_addition = once(add)

one_addition(<span class="integer">2</span>,<span class="integer">2</span>) <span class="comment"># 4</span>
one_addition(<span class="integer">2</span>,<span class="integer">2</span>) <span class="comment"># undefined</span>
one_addition(<span class="integer">12</span>,<span class="integer">200</span>) <span class="comment"># undefined</span>
</pre></div>
</div>

<h3>Super bonus</h3>

<p>Research what <code>decorators</code> are and refactor your <code>once</code> code to use a decorator so that you can run</p>
<div class="CodeRay">
  <div class="code"><pre><span class="decorator">@run_once</span>
<span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a+b

add(<span class="integer">2</span>,<span class="integer">2</span>) <span class="comment"># 4</span>
add(<span class="integer">2</span>,<span class="integer">20</span>) <span class="comment"># None</span>
add(<span class="integer">12</span>,<span class="integer">20</span>) <span class="comment"># None</span>
</pre></div>
</div>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_1_solutions/blob/master/python_functions/functions.py">here</a>.</p>

<h3>Part II</h3>

<p>Complete the following Codewars problems:</p>

<p><a target="_blank" href="https://www.codewars.com/kata/reversed-strings">Reversed Strings</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/looking-for-a-benefactor">Looking for a benefactor</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/sum-of-a-sequence/">Sum of a sequence</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/max-diff-easy-1/python">Max diff</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/583203e6eb35d7980400002a/">Count the similey faces!</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/sentence-count">Sentence Count</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/tortoise-racing">Tortoise Racing</a></p>

<p><a target="_blank" href="https://www.codewars.com/kata/calculate-string-rotation">Calculate String Rotation</a></p>

When you're ready, move on to Debugging Python

<h1>Debugging Python</h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Identify common errors in Python</li>
<li>Understand the causes of common errors in Python</li>
<li>Catch errors using <code>try</code> and <code>except</code></li>
<li>set break points in your Python code</li>
</ul>

<p>Just like in any programming language we learn, bugs are going to happen! As you&#39;ve probably noticed, in Python we have quite a few errors. Let&#39;s review some of the common ones:</p>

<h4><code>NameError</code></h4>

<p>This occurs when a variable is not defined:</p>
<div class="CodeRay">
  <div class="code"><pre>test
<span class="comment"># NameError: name 'test' is not defined</span>
</pre></div>
</div>

<h4><code>KeyError</code></h4>

<p>This occurs when a dictionary does not have a specific key:</p>
<div class="CodeRay">
  <div class="code"><pre>d = {}
d[<span class="string"><span class="delimiter">&quot;</span><span class="content">foo</span><span class="delimiter">&quot;</span></span>]
<span class="comment"># KeyError: 'foo'</span>
</pre></div>
</div>

<h4><code>AttributeError</code></h4>

<p>This occurs when a variable does not have an attribute:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>.foo
<span class="comment"># AttributeError: 'str' object has no attribute 'foo'</span>
</pre></div>
</div>

<h4><code>IndexError</code></h4>

<p>This occurs when you try to access an element in a list using an invalid index (i.e. one that is outside the range of the list):</p>
<div class="CodeRay">
  <div class="code"><pre>list = [<span class="string"><span class="delimiter">&quot;</span><span class="content">hello</span><span class="delimiter">&quot;</span></span>]
<span class="predefined">list</span>[<span class="integer">2</span>]
<span class="comment"># IndexError: list index out of range</span>
</pre></div>
</div>

<h4><code>ValueError</code></h4>

<p>This occurs when a built-in operation or function receives an argument that has the right type but an inappropriate value:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="predefined">int</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">foo</span><span class="delimiter">&quot;</span></span>)
<span class="comment"># ValueError: invalid literal for int() with base 10: 'foo'</span>
</pre></div>
</div>

<h4><code>TypeError</code></h4>

<p>This occurs when Python can not interpret two data types:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span> + [] <span class="comment"># TypeError: cannot concatenate 'str' and 'list' objects</span>
</pre></div>
</div>

<h3>raise</h3>

<p>In python we can also throw errors using the <code>raise</code> keyword. This is helpful when creating your own kinds of exception and error messages.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">raise</span> <span class="exception">ValueError</span>(<span class="string"><span class="delimiter">'</span><span class="content">invalid value</span><span class="delimiter">'</span></span>)
</pre></div>
</div>

<h3>try / except</h3>

<p>In Python, it is <strong>strongly</strong> encouraged to use <code>try/except</code> blocks, to catch exceptions when we can do something about them. Let&#39;s see what that looks like.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">try</span>: 
    foobar
<span class="keyword">except</span> <span class="exception">NameError</span> <span class="keyword">as</span> err:
    print(err)
</pre></div>
</div>

<p>We could also write something like this, but you should try not to. Why do you think someone might object to the following code?</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">try</span>: 
    nice + []
<span class="keyword">except</span>:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">Something went wrong!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>What we are doing here is catching <strong>every</strong> error, which means we are not able to correctly identify &quot;what&quot; went wrong. It is highly discouraged to do this. When you use <code>try/except</code>, make sure that a specific type of exception is being handled. If you want to except a handful of exceptions, you can pass a tuple of errors into the except block as well:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">try</span>:
    <span class="comment"># do some stuff</span>
<span class="keyword">except</span> (<span class="exception">NameError</span>, <span class="exception">ValueError</span>) <span class="keyword">as</span> e:
    <span class="comment"># do some other stuff</span>
</pre></div>
</div>

<h3>Debugging with <code>pdb</code></h3>

<p>To set breakpoints in our code we can use <code>pdb</code> by inserting this line:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">pdb</span>; pdb.set_trace() 
</pre></div>
</div>

<p>Inside of the debugger we can press <code>c</code> to continue and <code>q</code> to quit. There are a few more shortcuts as well; you can read more about <code>pdb</code> <a target="_blank" href="https://docs.python.org/2/library/pdb.html">here</a>.</p>

When you're ready, move on to Modules Introduction

<h1> Modules Introduction</h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Define what a module is </li>
<li>Import custom and built-in modules </li>
<li>Explain the purpose of the <code>if __name__ == &#39;__main__&#39;</code> pattern</li>
</ul>

<p>Python gives us a very nice way to import and export modules, which are pieces of code that we can encapsulate in their own files. </p>

<h3>Writing our own modules</h3>

<p>Let&#39;s start by writing our first module. This file is going to contain a few functions that we may want to use across several different Python files. Let&#39;s call this file <code>helpers.py</code></p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a + b

<span class="keyword">def</span> <span class="function">subtract</span>(a,b):
    <span class="keyword">return</span> a - b
</pre></div>
</div>

<p>Now in another Python file called <code>app.py</code> (in the same directory), let&#39;s import the helpers we just created:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">helpers</span> <span class="keyword">import</span> <span class="include">add</span>, <span class="include">subtract</span>

<span class="keyword">def</span> <span class="function">calculate_numbers</span>(a,b,fn):
    <span class="keyword">if</span> fn == <span class="string"><span class="delimiter">'</span><span class="content">add</span><span class="delimiter">'</span></span>:
        <span class="keyword">return</span> add(a,b)
    <span class="keyword">elif</span> fn == <span class="string"><span class="delimiter">'</span><span class="content">subtract</span><span class="delimiter">'</span></span>:
        <span class="keyword">return</span> subtract(a,b)

calculate_numbers(<span class="integer">1</span>, <span class="integer">4</span>, <span class="string"><span class="delimiter">'</span><span class="content">add</span><span class="delimiter">'</span></span>) <span class="comment"># this should work - we're able to access add from the helpers file!</span>
</pre></div>
</div>

<h3>The <code>import</code> keyword</h3>

<p>As you can see in the previous example, we grab code from other Python files using the <code>import</code> keyword. By convention, you should put your import statements at the top of your code. In general it&#39;s best to import what you need from the module rather than the entire module, but for some smaller built-in modules it doesn&#39;t matter too much.</p>

<p>Here are a few different ways to import the same thing and call it:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">random</span> <span class="comment"># importing everything from random</span>
<span class="comment"># when you import an entire module, functions exist as methods on that module</span>
random.random() <span class="comment"># generates a random number</span>
</pre></div>
</div>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">random</span> <span class="keyword">as</span> r <span class="comment"># importing everything, but aliasing it to a shorter variable</span>
r.random() <span class="comment"># generates a random number</span>
</pre></div>
</div>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">random</span> <span class="keyword">import</span> <span class="include">random</span> <span class="comment"># just importing the random function</span>
random() <span class="comment"># generates a random number - in this case, the function is just called on its own!</span>
</pre></div>
</div>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">random</span> <span class="keyword">import</span> <span class="include">random</span> <span class="keyword">as</span> r <span class="comment"># importing and aliasing just one function</span>
r() <span class="comment"># generates a random number</span>
</pre></div>
</div>

<p>Here are a few more <code>import</code> examples!</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">math</span> <span class="keyword">as</span> m <span class="comment"># importing everything from math, but aliasing math to the variable m</span>

<span class="keyword">from</span> <span class="include">math</span> <span class="keyword">import</span> <span class="include">sqrt</span> <span class="comment"># importing just the sqrt function from math</span>
<span class="keyword">from</span> <span class="include">my_module</span> <span class="keyword">import</span> <span class="include">*</span> <span class="comment"># importing everything from my_module</span>

<span class="keyword">import</span> <span class="include">my_second_module</span>
<span class="keyword">from</span> <span class="include">my_module</span> <span class="keyword">import</span> <span class="include">only_what_i_need</span>
</pre></div>
</div>

<h3><code>name == &#39;__main__&#39;</code></h3>

<p>One of the more common patterns you will see in Python modules is the following code </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">if</span> __name__ == <span class="string"><span class="delimiter">'</span><span class="content">__main__</span><span class="delimiter">'</span></span>:
    <span class="comment"># do something here</span>
</pre></div>
</div>

<p>The idea behind this code is that <code>__name__</code> is a special property of the file that will only be <code>__main__</code> when the file is loaded directly, rather than being imported. When modules are imported, all of the code inside of the module is run. However, there are times that we do not want code inside of a module to run when it is imported. In these cases, we can prevent code from running on import by checking the value of <code>__name__</code>. If <code>__name__</code> is equal to the string <code>&quot;__main__&quot;</code>, then the file has NOT been imported and is being run directly. </p>

<p>It&#39;s easiest to understand this by way of example. Let&#39;s create a <code>helper.py</code> file with the following code:</p>
<div class="CodeRay">
  <div class="code"><pre>print(<span class="string"><span class="delimiter">&quot;</span><span class="content">I'm from the helper file!</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">def</span> <span class="function">display</span>(name):
  print(<span class="string"><span class="delimiter">&quot;</span><span class="content">My name is </span><span class="delimiter">&quot;</span></span> + name)

display(__name__)  

<span class="keyword">if</span> __name__ == <span class="string"><span class="delimiter">'</span><span class="content">__main__</span><span class="delimiter">'</span></span>:
  print(<span class="string"><span class="delimiter">&quot;</span><span class="content">I'm the helper file and was loaded directly!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>If you run <code>python3 helper.py</code> in Terminal, you should see three lines printed to the terminal window. In particular, you should see that the <code>__name__</code> variable does indeed have the value of <code>__main__</code>.</p>

<p>But now let&#39;s see what happens when we import this file into another file, call it <code>other.py</code>:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">helper</span>

print(<span class="string"><span class="delimiter">&quot;</span><span class="content">I'm from the other file!</span><span class="delimiter">&quot;</span></span>)

helper.display(__name__)  

<span class="keyword">if</span> __name__ == <span class="string"><span class="delimiter">'</span><span class="content">__main__</span><span class="delimiter">'</span></span>:
  print(<span class="string"><span class="delimiter">&quot;</span><span class="content">I'm the other file and was loaded directly!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>When you run this file, you should see the following messages print:</p>
<div class="CodeRay">
  <div class="code"><pre>I'm from the helper file!
My name is helper
I'm from the other file!
My name is __main__
I'm the other file and was loaded directly!
</pre></div>
</div>

<p>Notice that in this case, the <code>__name__</code> variable inside of <code>helper.py</code> is just <code>&#39;helper&#39;</code>; because of this, the code inside of the <code>if __name__ == &#39;__main__&#39;</code> block doesn&#39;t run in that file! However, in <code>other.py</code>, <code>__name__</code> <em>does</em> equal <code>&#39;__main__&#39;</code>.</p>

<p>You can read more about this pattern <a target="_blank" href="https://www.quora.com/Why-would-you-use-if-__name__-__main__">here</a> or watch <a target="_blank" href="https://www.youtube.com/watch?v=sugvnHA7ElY">this</a> great tutorial.</p>
When you're ready, move on to Useful Python Modules

<h1>Useful Python Modules</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Distinguish between the different types of imports </li>
<li>Give examples of advanced data types provided by the <code>collections</code> module</li>
</ul>

<p>Now that you know how to import, let&#39;s examine a few useful modules:</p>

<h4>Random</h4>

<p>The <code>random</code> module is quite useful for generating random values of all kinds:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">random</span>

random.randint(<span class="integer">1</span>,<span class="integer">10</span>) <span class="comment"># generate a number between 1 and 10</span>
random.randrange(<span class="integer">4</span>) <span class="comment"># generate between 0 and 3</span>
random.random() <span class="comment"># generate a number between 0 and 1</span>
</pre></div>
</div>

<p>Here&#39;s an example pulling just a single function, the <code>choice</code> function, which grabs an element at random from a list:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">random</span> <span class="keyword">import</span> <span class="include">choice</span> <span class="keyword">as</span> c

c([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>]) <span class="comment"># run this line several times, you should see different elements get returned</span>
</pre></div>
</div>

<h4>Math</h4>

<p>The <code>math</code> module provides access to many mathematical functions, including helpers for rounding, constants like <code>e</code> and <code>pi</code>, and trigonometric functions.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">math</span>

math.e <span class="comment"># 2.718281828459045</span>
math.pi <span class="comment"># 3.141592653589793</span>
math.floor(<span class="float">2.2</span>) <span class="comment"># 2</span>
math.ceil(<span class="float">2.2</span>) <span class="comment"># 3</span>
math.sqrt(<span class="integer">16</span>) <span class="comment"># 4</span>
math.pow(<span class="integer">2</span>,<span class="integer">10</span>) <span class="comment"># 1024.0</span>
</pre></div>
</div>

<h3>Collections</h3>

<p>This is a built in module that provides alternatives to Python&#39;s built-in containers like <code>dict</code>, <code>list</code>, <code>set</code>, and <code>tuple</code>. Take a look at each one of these and see what they do.</p>

<h4>Counter</h4>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">collections</span> <span class="keyword">import</span> <span class="include">Counter</span>

l = [<span class="integer">1</span>,<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">4</span>,<span class="integer">5</span>,<span class="integer">5</span>]
Counter(l) <span class="comment"># see what this returns!</span>

string = <span class="string"><span class="delimiter">&quot;</span><span class="content">aweosakjdsaldwjdwq</span><span class="delimiter">&quot;</span></span>
Counter(string)

s = <span class="string"><span class="delimiter">'</span><span class="content">this is such a nice nice nice thing that is nice!</span><span class="delimiter">'</span></span>

c = Counter(s.split())

<span class="comment"># Counter({'a': 1,</span>
<span class="comment">#          'is': 2,</span>
<span class="comment">#          'nice': 3,</span>
<span class="comment">#          'nice!': 1,</span>
<span class="comment">#          'such': 1,</span>
<span class="comment">#          'that': 1,</span>
<span class="comment">#          'thing': 1,</span>
<span class="comment">#          'this': 1})</span>

c.items() <span class="comment"># list of element,count tuples </span>
c.clear() <span class="comment"># clear all values</span>
c.values() <span class="comment"># see all values</span>
</pre></div>
</div>

<h4>Defaultdict</h4>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">collections</span> <span class="keyword">import</span> <span class="include">defaultdict</span>

regular_dict = <span class="predefined">dict</span>(first=<span class="integer">1</span>)
regular_dict[<span class="string"><span class="delimiter">'</span><span class="content">first</span><span class="delimiter">'</span></span>] <span class="comment"># 1</span>
regular_dict[<span class="string"><span class="delimiter">'</span><span class="content">second</span><span class="delimiter">'</span></span>] <span class="comment"># KeyError!</span>

<span class="keyword">def</span> <span class="function">default_value</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">nothing</span><span class="delimiter">&quot;</span></span>

d = defaultdict(default_value)
d[<span class="string"><span class="delimiter">'</span><span class="content">nice</span><span class="delimiter">'</span></span>] = <span class="string"><span class="delimiter">&quot;</span><span class="content">cool</span><span class="delimiter">&quot;</span></span>
d[<span class="string"><span class="delimiter">'</span><span class="content">nice</span><span class="delimiter">'</span></span>] <span class="comment"># &quot;cool&quot;</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">whoaaa</span><span class="delimiter">'</span></span>] <span class="comment"># &quot;nothing&quot;</span>
</pre></div>
</div>

<h4>OrderedDict</h4>

<p>An ordered dictionary remembers the order in which key-value pairs were added.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">collections</span> <span class="keyword">import</span> <span class="include">OrderedDict</span>

d = {}
d[<span class="string"><span class="delimiter">'</span><span class="content">one</span><span class="delimiter">'</span></span>] = <span class="integer">1</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">two</span><span class="delimiter">'</span></span>] = <span class="integer">2</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">three</span><span class="delimiter">'</span></span>] = <span class="integer">3</span>
d[<span class="string"><span class="delimiter">'</span><span class="content">four</span><span class="delimiter">'</span></span>] = <span class="integer">4</span>

<span class="keyword">for</span> k,v <span class="keyword">in</span> d.items():
    print(k,v) <span class="comment"># no order!</span>

od = OrderedDict()
od[<span class="string"><span class="delimiter">'</span><span class="content">one</span><span class="delimiter">'</span></span>] = <span class="integer">1</span>
od[<span class="string"><span class="delimiter">'</span><span class="content">two</span><span class="delimiter">'</span></span>] = <span class="integer">2</span>
od[<span class="string"><span class="delimiter">'</span><span class="content">three</span><span class="delimiter">'</span></span>] = <span class="integer">3</span>
od[<span class="string"><span class="delimiter">'</span><span class="content">four</span><span class="delimiter">'</span></span>] = <span class="integer">4</span>

<span class="keyword">for</span> k,v <span class="keyword">in</span> od.items():
    print(k,v) <span class="comment"># order!</span>
</pre></div>
</div>

<h4>namedtuple</h4>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">collections</span> <span class="keyword">import</span> <span class="include">namedtuple</span>

t = (<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>)
t[<span class="integer">1</span>] = <span class="integer">2</span>

Person = namedtuple(<span class="string"><span class="delimiter">'</span><span class="content">Person</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">first_name last_name fav_color</span><span class="delimiter">'</span></span>)
elie = Person(<span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">Schoppik</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">purple</span><span class="delimiter">'</span></span>)
elie.fav_color <span class="comment"># 'purple'</span>
</pre></div>
</div>

When you're ready, move on to Debugging and Modules Exercises

<h1> Debugging and Modules Exercises</h1>

<ul>
<li>What is a module?</li>
<li>List three ways to import a module in Python.</li>
<li>What is the purpose of importing?</li>
<li>List three examples when you would use the <code>random</code> module.</li>
<li>What is an <code>ImportError</code>? </li>
<li>When would using an <code>OrderedDict</code> be useful?</li>
<li>When would using a <code>defaultdict</code> be useful?</li>
<li><p>What is the purpose of the following code:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">if</span> __name__ == <span class="string"><span class="delimiter">'</span><span class="content">__main__</span><span class="delimiter">'</span></span>:
    <span class="keyword">pass</span>
</pre></div>
</div></li>
</ul>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_1_solutions/blob/master/python_debugging_and_modules/solutions.md">here</a>.</p>

<h1>Introduction to Object Oriented Programming in Python. </h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Describe OOP without talking about code</li>
<li>Describe what encapsulation is</li>
<li>Describe what abstraction is</li>
<li>Create classes using Python</li>
<li>Write class and instance methods </li>
</ul>

<p>In Python 3, everything is an object! We can examine what kind of object using the <code>type()</code> function. We&#39;ve seen examples of this with built-in data types like booleans, strings, and integers. In this chapter, we&#39;ll create our own data types, in a way, using <em>classes</em>. Any instances of that class that we create will have a type equal to that class.</p>

<h3>What is Object Oriented Programming?</h3>

<p>Object oriented programming is a method of programming that attempts to model some process or thing in the world as a <strong>class</strong> or <strong>object</strong>. Conceptually, you can think of a class or object as something that has data and can perform operations on that data.  With object oriented programming, the goal is to <em>encapsulate</em> your code into logical groupings using classes so that you can reason about your code at a higher level. Before we get ahead of ourselves, though, let&#39;s define some terminology and see an example:</p>

<p><strong>Class</strong> - A blueprint for objects. Classes can contain methods and properties. We commonly use classes to reduce code duplication.  </p>

<p><strong>Instance</strong> - objects that are made from a class by calling the class. Instances share a similar structure because they all come from the same blueprint (i.e. class).</p>

<h3>Poker Example</h3>

<p>Say we want to model a game of poker in our program.  We could write the program using a list to represent the deck of cards, and then other lists to represent what each player has in their hand.  Then we&#39;d have to write a lot of functions to do things like deal, draw cards, see who wins, etc.</p>

<p>When you end up writing large functions and lots of code in one file, there is usually a better way to organize your code.  Instead of trying to do everything at once, we could <strong>separate concerns</strong>.</p>

<p>When thinking about a game of poker, some larger processes and objects stand out that you will want to capture in your code:</p>

<ul>
<li>Card</li>
<li>Deck of cards</li>
<li>Poker hand</li>
<li>Poker game</li>
<li>Discard pile (maybe)</li>
<li>Player</li>
<li>Bets</li>
</ul>

<p>Each one of these components could be a class in your program.  Let&#39;s pick one of the potential classes and figure out the data that it will hold and the functions that it should be able to perform:</p>

<p><strong>Deck of cards</strong></p>

<ul>
<li>Cards - the deck should have 52 different playing cards</li>
<li>Shuffle - the deck should be able to shuffle itself</li>
<li>Deal a card - remove a card from the deck and deal it to a player</li>
<li>Deal a hand - The deck may also be used to deal a hand to a player, or a set of players</li>
</ul>

<p>Now that we can conceptualize how a problem can be broken down into classes, let&#39;s talk about why programming this way can be useful.</p>

<h3>Encapsulation</h3>

<p>Encapsulation is the idea that data and processes on that data are owned by a class.  Other functions or classes outside of that class should not be able to directly change the data.</p>

<p>In our deck class, we have 52 cards. The player class should not be able to choose any card he or she wants from the deck or change the order of a deck manually.  Instead a player can only be dealt a hand.  The contents of the deck is said to be <em>encapsulated</em> into the deck class because the deck owns the list of cards and it will not allow other classes to access it directly.</p>

<h3>Abstraction</h3>

<p>Abstraction is the result of a good object oriented design.  Rather than thinking about the details of how a class works internally, you can think about it at a higher level.  You can see all of the functions that are made available by the class and understand what the class does without having to see all of the code or worry about implementation details.</p>

<p>Continuing with our example, if you had a deck of cards class and you saw that you could call the <code>.shuffle()</code> function or the <code>.deal()</code> function, you would have a good understanding of what the class does without having to understand how the functions are working internally.</p>

<p>Other hallmarks of object oriented programming include inheritance and polymorphism. We&#39;ll discuss these later.</p>

<h3>Creating a class</h3>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Vehicle</span>:
    <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,make,model,year):
        <span class="predefined-constant">self</span>.make = make
        <span class="predefined-constant">self</span>.model = model
        <span class="predefined-constant">self</span>.year = year
</pre></div>
</div>

<p>Every class needs an <code>__init__</code> method. Every time you create an instance from a class in Python, that instance will get run through the <code>__init__</code> method. <code>self</code> inside of this method refers to the instance.</p>

<p>To create an instance from a class, we instantiate the class using () and pass in the values to initialize the instance (these are defined in <code>__init__</code>).</p>
<div class="CodeRay">
  <div class="code"><pre>v = Vehicle(<span class="string"><span class="delimiter">'</span><span class="content">toyota</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">corolla</span><span class="delimiter">'</span></span>, <span class="integer">2012</span>)
</pre></div>
</div>

<h3>Methods and properties for instances</h3>

<p>To add methods on instances, we simply define them in the class. When defining instance methods, the first argument should always be called <code>self</code>, and refers to the current instance. If you need to pass other arguments, do so after passing in <code>self</code>. Note that when you call these instance methods, you never pass in <code>self</code>. Here are a couple of examples: </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Person</span>():

    <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>, first_name, last_name):
        <span class="predefined-constant">self</span>.first_name = first_name
        <span class="predefined-constant">self</span>.last_name = last_name

    <span class="keyword">def</span> <span class="function">full_name</span>(<span class="predefined-constant">self</span>):
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">My name is {} {}</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.first_name, <span class="predefined-constant">self</span>.last_name)

    <span class="keyword">def</span> <span class="function">likes</span>(<span class="predefined-constant">self</span>, thing):
          <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">{} likes {}!</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.first_name, thing)

p = Person(<span class="string"><span class="delimiter">'</span><span class="content">Tim</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">Garcia</span><span class="delimiter">'</span></span>)

p.full_name() <span class="comment"># My name is Tim Garcia</span>
p.likes(<span class="string"><span class="delimiter">&quot;</span><span class="content">computers</span><span class="delimiter">&quot;</span></span>) <span class="comment"># Tim likes computers!</span>
</pre></div>
</div>

<p>Notice that we <strong>must</strong> add <code>self</code> as the first parameter to each of our instance methods.</p>

<h3>Writing Class Methods</h3>

<p>We&#39;ve seen how to add methods on instances. But what if we want to add a method on the class itself? To do this, we use a decorator! We&#39;ll talk more about decorators later. For now, it&#39;s enough to know that there are two decorators we can use to create class methods:</p>

<p><strong>@classmethod</strong></p>

<p>One way use to use the <code>@classmethod</code> decorator:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Person</span>():

    <span class="decorator">@classmethod</span>
    <span class="keyword">def</span> <span class="function">say_hello</span>(cls):
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">HI!</span><span class="delimiter">&quot;</span></span>

Person.say_hello() <span class="comment"># &quot;HI!&quot;</span>
</pre></div>
</div>

<p>Similar to instance methods, the first argument in a class method has special meaning. For an instance method, the first argument refers to the instance, and is called <code>self</code>. For a class method, the first argument refers to the class, and is typically written as <code>cls</code>.</p>

<p><strong>@staticmethod</strong></p>

<p>Another decorator we can use is the <code>@staticmethod</code> decorator:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Person</span>():

    <span class="decorator">@staticmethod</span>
    <span class="keyword">def</span> <span class="function">say_hello</span>():
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">HI!</span><span class="delimiter">&quot;</span></span>

Person.say_hello() <span class="comment"># &quot;HI!&quot;</span>
</pre></div>
</div>

<p>So what are the differences between these two? See if you can spot it and head over <a target="_blank" href="http://stackoverflow.com/questions/136097/what-is-the-difference-between-staticmethod-and-classmethod-in-python">here</a> after!</p>

When you're ready, move on to Inheritance and MRO

<h1>Inheritance and MRO.</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Explain what inheritance is and how it is used to reduce code duplication</li>
<li>Understand what the <code>super</code> keyword does</li>
<li>Define MRO and explain how it is used in Python 3</li>
</ul>

<h3>Inheritance and <code>super</code></h3>

<p>In many languages that support object-oriented programming, you can define a class which inherits from another class. Python takes things even further; in Python, we can do what is called multiple inheritance. This means that one class can inherit from many other classes! </p>

<p>Here&#39;s an example of single inheritance: </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Vehicle</span>:
    <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,make,model,year):
        <span class="predefined-constant">self</span>.make = make
        <span class="predefined-constant">self</span>.model = model
        <span class="predefined-constant">self</span>.year = year
    <span class="keyword">def</span> <span class="function">honk</span>(<span class="predefined-constant">self</span>):
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">Beep!</span><span class="delimiter">&quot;</span></span>

<span class="keyword">class</span> <span class="class">Car</span>(Vehicle):
    <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,make,model,year):
        <span class="predefined">super</span>().__init__(make,model,year) <span class="comment"># this is python3 specific!</span>
        <span class="predefined-constant">self</span>.wheels = <span class="integer">4</span>
</pre></div>
</div>

<p>Notice that when we define the <code>Car</code> class, we pass in the <code>Vehicle</code> class. Then, inside of the car&#39;s <code>__init__</code> method we make a call to <code>super().__init__</code>, which refers to the parent class&#39;s <code>__init__</code> method. Calling <code>super</code> in this way ensures that car instances are assigned a <code>make</code>, <code>model</code>, and <code>year</code>, but saves us from having to repeat ourselves in the logic for the <code>Car</code>&#39;s <code>__init__</code> method.</p>

<p>Inheritance also saves us from having to duplicate instance methods: instances of the child class automatically gain access to instance methods in the parent class. Take a look:</p>
<div class="CodeRay">
  <div class="code"><pre>mack_truck = Vehicle(<span class="string"><span class="delimiter">&quot;</span><span class="content">Mack</span><span class="delimiter">&quot;</span></span>,<span class="string"><span class="delimiter">&quot;</span><span class="content">Titan</span><span class="delimiter">&quot;</span></span>,<span class="integer">2015</span>)
car = Car(<span class="string"><span class="delimiter">&quot;</span><span class="content">Honda</span><span class="delimiter">&quot;</span></span>,<span class="string"><span class="delimiter">&quot;</span><span class="content">Civic</span><span class="delimiter">&quot;</span></span>,<span class="integer">2004</span>)

mack_truck.honk() <span class="comment"># &quot;Beep!&quot;</span>
car.honk() <span class="comment"># &quot;Beep!&quot;</span>
</pre></div>
</div>

<p>In this case, we don&#39;t need to define a <code>honk</code> method for cars. Since the <code>Car</code> class inherits from <code>Vehicle</code>, any car instances will automatically have access to the <code>honk</code> method from the <code>Vehicle</code> class.</p>

<h3>Multiple Inheritance and MRO</h3>

<p>The car and vehicle example is fine when we want a class to inherit from one other class. But what if we want it to inherit from multiple classes? In this case, Python lets us do multiple inheritance by passing in multiple classes when we create a new class! Here&#39;s an example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Aquatic</span>:
  <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,name):
    <span class="predefined-constant">self</span>.name = name

  <span class="keyword">def</span> <span class="function">swim</span>(<span class="predefined-constant">self</span>):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">{} is swimming</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.name)

  <span class="keyword">def</span> <span class="function">greet</span>(<span class="predefined-constant">self</span>):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">I am {} of the sea!</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.name)

<span class="keyword">class</span> <span class="class">Ambulatory</span>:
  <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,name):
    <span class="predefined-constant">self</span>.name = name

  <span class="keyword">def</span> <span class="function">walk</span>(<span class="predefined-constant">self</span>):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">{} is walking</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.name)

  <span class="keyword">def</span> <span class="function">greet</span>(<span class="predefined-constant">self</span>):
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">I am {} of the land!</span><span class="delimiter">&quot;</span></span>.format(<span class="predefined-constant">self</span>.name)

<span class="keyword">class</span> <span class="class">Penguin</span>(Aquatic, Ambulatory):
  <span class="keyword">def</span> <span class="function">__init__</span>(<span class="predefined-constant">self</span>,name):
    <span class="predefined">super</span>().__init__(name=name) 

jaws = Aquatic(<span class="string"><span class="delimiter">&quot;</span><span class="content">Jaws</span><span class="delimiter">&quot;</span></span>)
lassie = Ambulatory(<span class="string"><span class="delimiter">&quot;</span><span class="content">Lassie</span><span class="delimiter">&quot;</span></span>)
captain_cook = Penguin(<span class="string"><span class="delimiter">&quot;</span><span class="content">Captain Cook</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>Here we define two classes: <code>Aquatic</code> (for things that can swim) and <code>Ambulatory</code> (for things that can walk). Instances of the <code>Aquatic</code> class have a <code>name</code>, a <code>swim</code> method, and a <code>greet</code> method. Similarly, instances of the <code>Ambulatory</code> class have a <code>name</code>, a <code>walk</code> method, and a <code>greet</code> method.</p>

<p>We then define a third class called <code>Penguin</code>, which inherits from both <code>Aquatic</code> and <code>Ambulatory</code>. Finally, we create an instance from each of these classes.</p>

<p>Let&#39;s examine what happens when we try to call methods on each of these instances. You should see the following:</p>
<div class="CodeRay">
  <div class="code"><pre>jaws.swim() <span class="comment"># 'Jaws is swimming'</span>
jaws.walk() <span class="comment"># AttributeError: 'Aquatic' object has no attribute 'walk'</span>
jaws.greet() <span class="comment"># 'I am Jaws of the sea!'</span>

lassie.swim() <span class="comment"># AttributeError: 'Ambulatory' object has no attribute 'swim'</span>
lassie.walk() <span class="comment"># 'Lassie is walking'</span>
lassie.greet() <span class="comment"># 'I am Lassie of the land!'</span>

captain_cook.swim() <span class="comment"># 'Captain Cook is swimming'</span>
captain_cook.walk() <span class="comment"># 'Captain Cook is walking'</span>
captain_cook.greet() <span class="comment"># 'I am Captain Cook of the sea!'</span>
</pre></div>
</div>

<p>Notice that because <code>Penguin</code> inherits from both <code>Aquatic</code> and <code>Ambulatory</code>, instances of the <code>Penguin</code> class have access to both the <code>swim</code> method and the <code>walk</code> method. </p>

<p>What happens with the <code>greet</code> method, though? In this case, there&#39;s a conflict, since both <code>Aquatic</code> and <code>Ambulatory</code> have their own <code>greet</code> methods! In this case, it looks like <code>Penguin</code> inherits the <code>greet</code> method from <code>Aquatic</code> and ignores the <code>greet</code> method from <code>Ambulatory</code>. (Notice that when we defined <code>Penguin</code>, we passed in <code>Aquatic</code> first, and then <code>Ambulatory</code>; what happens if you switch the order?)</p>

<p>So how does Python know where to search for methods? Whenever you create a class, Python sets a <strong>M</strong>ethod <strong>R</strong>esolution <strong>O</strong>rder, or MRO, for that class. This order determines the order in which Python will look for methods on instances of that class. With single inheritance (or even simple examples of multiple inheritance) the order isn&#39;t so hard to deduce, but for really complex multiple inheritance things can get tricky. If you ever need to see what the MRO is for a class, you can take a look at the <code>__mro__</code> attribute for that class, use the <code>mro()</code> method, or, even better, get some <code>help</code>:</p>
<div class="CodeRay">
  <div class="code"><pre>Penguin.__mro__ <span class="comment"># (&lt;class 'multiple.Penguin'&gt;, &lt;class 'multiple.Aquatic'&gt;, &lt;class 'multiple.Ambulatory'&gt;, &lt;class 'object'&gt;)</span>

<span class="comment"># OR</span>

Penguin.mro() <span class="comment"># returns a list to us</span>

<span class="comment"># EVEN BETTER!</span>

help(Penguin) <span class="comment"># gives us a detailed chain </span>
</pre></div>
</div>

When you're ready, move on to Special Methods and Polymorphism

<h1>Special Methods and Polymorphism</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Add special methods to classes</li>
<li>Define and explain how to implement polymorphism in a class</li>
<li>Understand how to add custom properties and methods to built in data types in Python</li>
</ul>

<h3>Special methods for python objects</h3>

<p>When we discuss special (also called &quot;magic&quot;) methods, we are commonly referring to methods that contain a &quot;dunder&quot; (double underscore) like <code>__init__</code>. You have actually used quite a few of these under the hood, but you can implement your own for classes you create. Let&#39;s see a couple:</p>

<p><code>__str__</code> - what is evaluated when <code>print</code> is called</p>

<p><code>__len__</code> - what is evaluated when <code>len</code> is called</p>

<p><code>__del__</code> - what is evaluated when <code>del</code> is called</p>

<p><code>__doc__</code> - see the docstring for a value</p>

<p><code>__class__</code> - see what class created this object</p>

<p>There also exists another method called <code>__repr__</code> which is similar to <code>__str__</code>; you can read about the differences <a target="_blank" href="http://stackoverflow.com/questions/1436703/difference-between-str-and-repr-in-python">here</a></p>

<p>You can read more about these <a target="_blank" href="http://www.diveintopython3.net/special-method-names.html">here</a>. Pay close attention to the differences between <code>__repr__</code>, <code>__str__</code> and <code>__format__</code></p>

<h3>Polymorphism</h3>

<p>One of the key principles in Object Oriented Programming is <em>polymorphism</em>. This is the idea that an object can take on many (poly) forms (morph).</p>

<p>A very common example you will see of Polymorphism is the <code>+</code> operator. If we do <code>5 + 3</code> in Python our result will be 8 as the operator knows to add the two numbers. But if we do <code>&quot;8&quot; + &quot;3&quot;</code> Python knows to concatenate the values since they are strings. This single operator can take on many different forms, depending on the types it is working with! </p>

<p>You can see polymorphism applied when there is the same operation used for objects in different classes. Let&#39;s see another example!</p>
<div class="CodeRay">
  <div class="code"><pre>sample_list = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>]
sample_tuple = (<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>)
sample_string = <span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>

<span class="predefined">len</span>(sample_list)
<span class="predefined">len</span>(sample_tuple)
<span class="predefined">len</span>(sample_string)
</pre></div>
</div>

<p>These are three different classes that have the same operation applied to them!</p>

<p>A common implementation of this is to have a method in a base (or parent) class that is overriden by a subclass. Each subclass will have a different implementation of the method. When the superclass/parent class method is called, it chooses which method to run depending on the subclass/child class. Let&#39;s look at a common example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">class</span> <span class="class">Pet</span>():
    <span class="keyword">def</span> <span class="function">talk</span>:
        <span class="keyword">raise</span> <span class="exception">NotImplementedError</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">Subclass needs to implement this method</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">class</span> <span class="class">Dog</span>(Pet):
    <span class="keyword">def</span> <span class="function">talk</span>(<span class="predefined-constant">self</span>):
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">WOOF!</span><span class="delimiter">&quot;</span></span>

<span class="keyword">class</span> <span class="class">Cat</span>(Pet):
    <span class="keyword">def</span> <span class="function">talk</span>(<span class="predefined-constant">self</span>):
        <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">MEOW!</span><span class="delimiter">&quot;</span></span>
</pre></div>
</div>

<p>To implement polymorphism you do not <strong>need</strong> a superclass / parent class. It is only when you are using inheritance and polymorphism together that it is useful to ensure that the subclass implements its own version of the method.</p>

<p>For more on polymorphism, check out these articles:</p>

<p><a target="_blank" href="http://blog.thedigitalcatonline.com/blog/2014/08/21/python-3-oop-part-4-polymorphism/#.WBD-PuErLEY">http://blog.thedigitalcatonline.com/blog/2014/08/21/python-3-oop-part-4-polymorphism/#.WBD-PuErLEY</a></p>

<p><a target="_blank" href="https://pythonspot.com/en/polymorphism/">https://pythonspot.com/en/polymorphism/</a></p>

<p><a target="_blank" href="http://stackoverflow.com/questions/409969/polymorphism-define-in-just-two-sentences">http://stackoverflow.com/questions/409969/polymorphism-define-in-just-two-sentences</a></p>

<h3>Add custom properties / methods to built in data types in Python</h3>

<p>In Python, you can&#39;t manipulate base classes for native data types in the same way. However, you can create a new class which extends the built in class, and add methods to the class you&#39;ve created. To do this, you&#39;ll need to import the <code>builtins</code> module and manipulate the class you&#39;re interested in. </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">builtins</span>

<span class="comment"># Extended subclass</span>
<span class="keyword">class</span> <span class="class">extend_str</span>(<span class="predefined">str</span>):
    <span class="keyword">def</span> <span class="function">first_last_character</span>(<span class="predefined-constant">self</span>):
        <span class="keyword">return</span> <span class="predefined-constant">self</span>[<span class="integer">0</span>] + <span class="predefined-constant">self</span>[-<span class="integer">1</span>]

<span class="comment"># Overwrite the str class on builtins with the custom class defined above</span>
builtins.str = extend_str

<span class="predefined">str</span>(<span class="octal">0123</span>).first_last_character() <span class="comment"># '03'</span>

<span class="predefined">str</span>(<span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>).first_last_character() <span class="comment"># 'ae'</span>

<span class="string"><span class="delimiter">&quot;</span><span class="content">awesome</span><span class="delimiter">&quot;</span></span>.first_last_character() <span class="comment"># 'str' object has no attribute 'first_last_character'</span>
</pre></div>
</div>

<p>Note that in the example above, you can&#39;t use your custom method on strings unless they&#39;re explicitly created by being passed into the <code>str</code> class. In short, this approach is cumbersome and not foolproof. But that&#39;s probably by design: you shouldn&#39;t be trying to modify these classes in the first place!</p>

When you're ready, move on to Object Oriented Programming in Python Exercises

<h1> Object Oriented Programming in Python Exercises
</h1>

 <h3>Part 1</h3>

<p>Answer the following questions.</p>

<ul>
<li>What is a class?</li>
<li>What is an instance?</li>
<li>What is encapsulation?</li>
<li>What is abstraction?</li>
<li>What is inheritance?</li>
<li>What is multiple inheritance?</li>
<li>What is polymorphism?</li>
<li>What is <code>method resolution order</code> or <code>MRO</code>?</li>
</ul>

<h3>Part 2</h3>

<p>Create a deck of cards class.  Internally, the deck of cards should use another class, a card class.  Your requirements are:</p>

<ul>
<li>The <code>Deck</code> class should have a <code>deal</code> method to deal a single card from the deck</li>
<li>After a card is dealt, it is removed from the deck.</li>
<li>There should be a <code>shuffle</code> method which makes sure the deck of cards has all 52 cards and then rearranges them randomly.</li>
<li>The <code>Card</code> class should have a suit (Hearts, Diamonds, Clubs, Spades) and a value (A,2,3,4,5,6,7,8,9,10,J,Q,K)</li>
</ul>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_2_solutions/tree/master/object_oriented_programming_with_python">here</a>.</p>

When you're ready, move on to File I/O Introduction

<h1>File I/O Introduction
</h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Read and write to text files</li>
<li>Explain the purpose of a <code>with</code> statement</li>
<li>Explain the different ways to open a file depending on whether you want to read, write, or append</li>
</ul>

<h3>Definitions</h3>

<p>Python has a lot of functionality to help you manipulate text files. In this chapter we&#39;ll explore some of this functionality. Before we do so, here are three terms you should know, as we&#39;ll be using them frequently when discussing file IO (input/output).</p>

<p><strong>Reading</strong> - Getting data from a file.  The data can be stored and manipulated in your program.</p>

<p><strong>Writing</strong> - Saving new data to a file.</p>

<p><strong>Cursor</strong> - When you read a file, a cursor gets created (just like a cursor when you are typing). You can&#39;t see this cursor, but this is how you can tell a file where to start reading from. Once the cursor is at the end of a file, you can not read it anymore unless you explicitly go back to the beginning</p>

<h3>Reading</h3>

<p>Let&#39;s start by creating a text file called <code>first.txt</code> and placing the following text inside of it:</p>
<div class="CodeRay">
  <div class="code"><pre>This is a very simple text file!
</pre></div>
</div>

<p>Now let&#39;s make a file called <code>read.py</code> and add the following.</p>
<div class="CodeRay">
  <div class="code"><pre>file = <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r</span><span class="delimiter">'</span></span>)
print(<span class="predefined">file</span>.read())
</pre></div>
</div>

<p>We just opened a file called <code>first.txt</code> for reading (that&#39;s what the second argument of <code>&#39;r&#39;</code> indicates). After opening the file and storing it in a variable called <code>file</code>, we call the <code>read</code> function on it, which allows us to move our cursor from the beginning to the end. Finally, we&#39;re not just reading the file; we&#39;re printing out the results of that read operation. If you run <code>python3 read.py</code> in Terminal (from the directory where <code>read.py</code> lives), you should see the text of the file in the terminal!</p>

<p>If we try to make invoke <code>file.read()</code> a second time, we just get an empty string back. This is because the cursor is at the end of the file and there is no more to read. In order to read the file again, we&#39;ll need to go back to the beginning of the file using <code>seek</code>. Hop into the Python REPL by typing <code>python3</code> in the terminal, then execute the following code:</p>
<div class="CodeRay">
  <div class="code"><pre>file = <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r</span><span class="delimiter">'</span></span>)

<span class="comment"># type in the following commands</span>

<span class="predefined">file</span>.read() <span class="comment"># we see all our test</span>
<span class="predefined">file</span>.read() <span class="comment"># nothing now!</span>

<span class="predefined">file</span>.seek(<span class="integer">0</span>) <span class="comment"># move the cursor back to the beginning</span>
<span class="predefined">file</span>.read() <span class="comment"># there it is!</span>
</pre></div>
</div>

<p>But we&#39;re not done yet, if we look at <code>file.closed</code> we will see the value is <code>False</code>. So we opened our file, but we never closed it! Let&#39;s always make sure we close the file!</p>
<div class="CodeRay">
  <div class="code"><pre>file = <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r</span><span class="delimiter">'</span></span>)

<span class="comment"># type in the following commands</span>

<span class="predefined">file</span>.read() <span class="comment"># we see all our test</span>
<span class="predefined">file</span>.read() <span class="comment"># nothing now!</span>

<span class="predefined">file</span>.seek(<span class="integer">0</span>) <span class="comment"># move the cursor back to the beginning</span>
<span class="predefined">file</span>.read() <span class="comment"># there it is!</span>

<span class="predefined">file</span>.closed <span class="comment"># False</span>
<span class="predefined">file</span>.close()
<span class="predefined">file</span>.closed <span class="comment"># True</span>

<span class="predefined">file</span>.read() <span class="comment"># ValueError: I/O operation on closed file</span>
</pre></div>
</div>

<p>Note: for multiline files, you can read one line at a time using the <code>readline</code> method.</p>

<h3>keyword <code>with</code></h3>

<p>Instead of worrying about closing the file each time, we can use a <code>with</code> block, which will automatically close the file after the operation. Let&#39;s see what that looks like:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    data = <span class="predefined">file</span>.read()
    print(data)

<span class="predefined">file</span>.closed <span class="comment"># True</span>
</pre></div>
</div>

<h3>Writing</h3>

<p>In the previous examples, we&#39;ve seen that the <code>open</code> function takes two parameters. The first is the path to the text file. But what&#39;s the second? Here is where we tell Python what we intend to do with the file. Here are the options for what we can pass in:</p>

<ul>
<li><code>r</code> use this when you only want to read the file.</li>
<li><code>r+</code> use this when you want to read and write to the file. In this case, if you write to the file, you&#39;ll overwrite any existing characters while you&#39;re writing based on the location of the cursor, but once you&#39;ve finished writing, other characters will be unaffected.</li>
<li><code>a</code> use this when you want to <em>append</em> to the file (text that&#39;s already in the file won&#39;t be affected)</li>
<li><code>a+</code> use this when you want to read the file and append to it.</li>
<li><code>w</code> use this when you want to <em>write</em> to the file. In this case, the file is completely emptied before it&#39;s written to, so the original text data will be lost.</li>
<li><code>w+</code> use this when you want to write and read to the file.</li>
</ul>

<p>If you don&#39;t pass anything in to the second argument to <code>open</code>, <code>r</code> will be assumed.</p>

<p>Take a look at these examples to see how these options behave differently:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">w</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    <span class="predefined">file</span>.write(<span class="string"><span class="delimiter">'</span><span class="content">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Eos molestias ea sit veniam, rerum, totam quis eaque excepturi aut, nostrum reiciendis. At, harum quos adipisci magni nesciunt aliquid beatae sit!</span><span class="delimiter">'</span></span>)

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    print(<span class="predefined">file</span>.read())

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">r+</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    <span class="predefined">file</span>.write(<span class="string"><span class="delimiter">&quot;</span><span class="char">\n</span><span class="content">I'm at the beginning</span><span class="char">\n</span><span class="delimiter">&quot;</span></span>)
    <span class="predefined">file</span>.seek(<span class="integer">100</span>)
    <span class="predefined">file</span>.write(<span class="string"><span class="delimiter">&quot;</span><span class="char">\n</span><span class="content">I'm in the middle</span><span class="char">\n</span><span class="delimiter">&quot;</span></span>)
    <span class="predefined">file</span>.seek(<span class="integer">0</span>)
    print(<span class="predefined">file</span>.read())

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">a+</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    <span class="predefined">file</span>.write(<span class="string"><span class="delimiter">&quot;</span><span class="char">\n</span><span class="content">I'm at the end</span><span class="char">\n</span><span class="delimiter">&quot;</span></span>)
    <span class="predefined">file</span>.seek(<span class="integer">0</span>)
    print(<span class="predefined">file</span>.read())

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">first.txt</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">w+</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> <span class="predefined">file</span>:
    <span class="predefined">file</span>.write(<span class="string"><span class="delimiter">&quot;</span><span class="content">Now everything is overwritten :(</span><span class="delimiter">&quot;</span></span>)
    <span class="predefined">file</span>.seek(<span class="integer">0</span>)
    print(<span class="predefined">file</span>.read())
</pre></div>
</div>

When you're ready, move on to File I/O with CSVs

<h1> File I/O with CSVs</h1>

<h3>Objectives:</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Explain what a CSV file is</li>
<li>Read and write to CSV files</li>
</ul>

<h3>CSV with Python</h3>

<p>Aside from reading text files, we can also read <code>csv</code>, or comma separated values. CSV files can be opened in a text editor or more commonly in programs like Microsoft Excel. CSVs are a common format for uploading and downloading data, so understanding how to programmatically work with them is important. Here is an example <code>csv</code> file:</p>

<p><code>pets.csv</code></p>
<div class="CodeRay">
  <div class="code"><pre>name,type,age
Whiskey,dog,3
Moxie,cat,7
Mascis,dog,2
</pre></div>
</div>

<p>Most languages can actually support files that are separated by any character, not just commas (there is another format called <code>tsv</code> for tab separated values).  Here is an example of a file that is separated by <code>|</code> (we call the character we separate by the &quot;delimiter&quot;):</p>

<p><code>file.csv</code></p>
<div class="CodeRay">
  <div class="code"><pre>name|type|age
Whiskey|dog|3
Moxie|cat|7
Mascis|dog|2
</pre></div>
</div>

<p>Now, to read <code>csv</code> files, we&#39;ll need to import the <code>csv</code> module and use the <code>csv.reader</code> method. Let&#39;s take a look at an example.</p>

<p>Notice that the file we are reading in the example below,<code>file.csv</code>, is separated by <code>|</code>. Our next step is to read this file using the <code>csv</code> module:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">csv</span>

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">file.csv</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> csvfile:
    reader = csv.reader(csvfile, delimiter=<span class="string"><span class="delimiter">'</span><span class="content">|</span><span class="delimiter">'</span></span>)
    rows = <span class="predefined">list</span>(reader)
    <span class="keyword">for</span> row <span class="keyword">in</span> rows:
        print(<span class="string"><span class="delimiter">'</span><span class="content">, </span><span class="delimiter">'</span></span>.join(row))

<span class="comment"># name, type, age</span>
<span class="comment"># Whiskey, dog, 3</span>
<span class="comment"># Moxie, cat, 7</span>
<span class="comment"># Mascis, dog, 2</span>
</pre></div>
</div>

<p>We can also create a dictionary for each row instead of a list, if we use the <code>DictReader</code> method:     </p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">csv</span>

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">file.csv</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> csvfile:
    reader = csv.DictReader(csvfile, delimiter=<span class="string"><span class="delimiter">'</span><span class="content">|</span><span class="delimiter">'</span></span>)
    rows = <span class="predefined">list</span>(reader)
    <span class="keyword">for</span> row <span class="keyword">in</span> rows:
        print(row)

<span class="comment"># {'age': '3', 'name': 'Whiskey', 'type': 'dog'}</span>
<span class="comment"># {'age': '7', 'name': 'Moxie', 'type': 'cat'}</span>
<span class="comment"># {'age': '2', 'name': 'Mascis', 'type': 'dog'}        </span>
</pre></div>
</div>

<p>Finally, we can also write to <code>csv</code> files in a similar way that we write to plain text files. But rather than creating a <code>reader</code>, you&#39;ll need to create a <code>writer</code>:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">file.csv</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> csvfile:
    data_writer = csv.writer(csvfile, delimiter=<span class="string"><span class="delimiter">&quot;</span><span class="content">|</span><span class="delimiter">&quot;</span></span>)
    data_writer.writerow([<span class="string"><span class="delimiter">'</span><span class="content">Bojack</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">Horse</span><span class="delimiter">'</span></span>,<span class="string"><span class="delimiter">'</span><span class="content">50</span><span class="delimiter">'</span></span>])
</pre></div>
</div>

<p>As before, you can also write using dictionaries instead of lists. Here&#39;s an example for a new <code>csv</code> that we&#39;re building from scratch.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">newfile.csv</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">a</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> csvfile:
    data = [<span class="string"><span class="delimiter">'</span><span class="content">name</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">fav_topic</span><span class="delimiter">'</span></span>]
    writer = csv.DictWriter(csvfile, fieldnames=data)
    writer.writeheader() <span class="comment"># this writes the first row with the column headings</span>
    writer.writerow({
        <span class="string"><span class="delimiter">'</span><span class="content">name</span><span class="delimiter">'</span></span>: <span class="string"><span class="delimiter">'</span><span class="content">Elie</span><span class="delimiter">'</span></span>,
        <span class="string"><span class="delimiter">'</span><span class="content">fav_topic</span><span class="delimiter">'</span></span>: <span class="string"><span class="delimiter">'</span><span class="content">Writing to CSVs!</span><span class="delimiter">'</span></span>     
    }) 
</pre></div>
</div>

<p>To learn more about working with CSVs in Python, you know what to do: check the <a target="_blank" href="https://docs.python.org/3.0/library/csv.html">docs</a>!</p>

When you're ready, move on to File I/O Exercises

<h1>File I/O Exercises
</h1>

<h3>Part 1 - Text Files</h3>

<p>For the first part of this exercise assume you have a file called <code>students.txt</code> which simply contains a bunch of student names, one name per line. Your goal is to write two functions:</p>

<ul>
<li><code>add_student</code> - accepts a parameter of <code>first_name</code> and writes to a file called <code>students.txt</code>. </li>
<li><code>find_student</code> - accepts a parameter of <code>first_name</code> and returns the first student found</li>
</ul>

<h4>Bonuses</h4>

<ol>
<li>Write the following additional functions:

<ul>
<li><code>update_student</code> - accepts a parameter of <code>first_name</code> and <code>new_name</code> and updates first student found</li>
<li><code>remove_student</code> - accepts a parameter of <code>first_name</code> and removes the student from the text file</li>
</ul></li>
<li>Add a unique id for each student so that you can find a student by their id instead of first name (which breaks if you have the same first name for multiple students)</li>
</ol>

<h3>Part 2 - CSV</h3>

<p>For the next part of this exercise, you will be working with CSVs, so first create a file called <code>users.csv</code> and then work on the following two functions: </p>

<ul>
<li>one that prints out all of the first and last names in the <code>users.csv</code> file</li>
<li>one that prompts us to enter a first and last name and adds it to the <code>users.csv</code> file. </li>
</ul>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_2_solutions/tree/master/file_io">here</a>.</p>

When you're ready, move on to Generators and Iterators

<h1> Generators and Iterators</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Explain what a generator is and how to create one in Python</li>
<li>Understand what the <code>yield</code> keyword and <code>next</code> function do</li>
<li>Define and create iterators using the <code>iter</code> function</li>
<li>Access values and indexes using <code>enumerate</code></li>
</ul>

<h3>Generators</h3>

<p>Generator functions are functions that allow us to return multiple times using the <code>yield</code> keyword. This allows us to generate many values over time from a single function. What makes generators so powerful is that unlike other forms of iteration, the values are not all computed upfront so we can suspend our state using the <code>yield</code> keyword and come back to to the function later to continue on. This makes generators a great choice for things like calculating large data sets.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">gensquares</span>(n):
    <span class="keyword">for</span> num <span class="keyword">in</span> <span class="predefined">range</span>(n):
        <span class="keyword">yield</span> num**<span class="integer">2</span>

<span class="keyword">for</span> x <span class="keyword">in</span> gensquares(<span class="integer">10</span>):
    print(x)
</pre></div>
</div>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">fib_with_generator</span>(n):
    a = <span class="integer">1</span>
    b = <span class="integer">1</span>
    <span class="keyword">for</span> i <span class="keyword">in</span> <span class="predefined">range</span>(n):
        <span class="keyword">yield</span> a
        <span class="comment"># a,b = b, a+b -&gt; tuple unpacking instead of the three lines below!</span>
        temp = a
        a = b
        b = temp+b

<span class="keyword">for</span> num <span class="keyword">in</span> fib_with_generator(<span class="integer">10</span>):
    print(num)
</pre></div>
</div>

<h3>Using the <code>next</code> function</h3>

<p>Given a generator, you can obtain the next value by calling a special function called <code>next</code> and passing in the generator. Here&#39;s an example:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">use_next</span>():
    <span class="keyword">for</span> x <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">10</span>):
        <span class="keyword">yield</span> x

gen = use_next()
print(<span class="predefined">next</span>(gen)) <span class="comment"># 0</span>
print(<span class="predefined">next</span>(gen)) <span class="comment"># 1</span>
print(<span class="predefined">next</span>(gen)) <span class="comment"># 2</span>
</pre></div>
</div>

<p>In the example above, you can&#39;t call next infinitely many times: eventually you&#39;ll get a <code>StopIteration</code> error (since <code>x</code> inside of <code>use_next</code> only has finitely many values).</p>

<p>However, if you iterate through a generator using something like a <code>for</code> loop, the loop will catch the error so that it doesn&#39;t break your program:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">for</span> val <span class="keyword">in</span> use_next():
    print(val)

<span class="comment"># 0</span>
<span class="comment"># 1</span>
<span class="comment"># 2</span>
<span class="comment"># 3</span>
<span class="comment"># 4</span>
<span class="comment"># 5</span>
<span class="comment"># 6</span>
<span class="comment"># 7</span>
<span class="comment"># 8</span>
<span class="comment"># 9</span>
</pre></div>
</div>

<p>We can also do generator comprehension just like list comprehension by wrapping our comprehension in <code>()</code> to write generator functions with more ease. Here&#39;s how <code>use_next</code> would look as a generator comprehension:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">use_next</span>():
    <span class="keyword">return</span> (x <span class="keyword">for</span> x <span class="keyword">in</span> <span class="predefined">range</span>(<span class="integer">10</span>))
</pre></div>
</div>

<p>You can learn more about generators with these three resources: </p>

<p><a target="_blank" href="http://asmeurer.github.io/python3-presentation/python3-presentation.pdf">http://asmeurer.github.io/python3-presentation/python3-presentation.pdf</a></p>

<p><a target="_blank" href="http://stackoverflow.com/questions/1756096/understanding-generators-in-python">http://stackoverflow.com/questions/1756096/understanding-generators-in-python</a></p>

<p><a target="_blank" href="http://stackoverflow.com/questions/231767/what-does-the-yield-keyword-do-in-python?rq=1">(http://stackoverflow.com/questions/231767/what-does-the-yield-keyword-do-in-python?rq=1</a> </p>

<h3>Iterators</h3>

<p>To make something an iterable (i.e. something you can iterate over) we call the <code>iter</code> function on it. For example, if we wanted strings to be iterators, we could do:</p>
<div class="CodeRay">
  <div class="code"><pre>str = <span class="string"><span class="delimiter">&quot;</span><span class="content">hello</span><span class="delimiter">&quot;</span></span>
str_iter = <span class="predefined">iter</span>(<span class="predefined">str</span>)
<span class="predefined">next</span>(str_iter) <span class="comment"># h</span>
<span class="predefined">next</span>(str_iter) <span class="comment"># e</span>
<span class="predefined">next</span>(str_iter) <span class="comment"># l</span>
<span class="predefined">next</span>(str_iter) <span class="comment"># l</span>
<span class="predefined">next</span>(str_iter) <span class="comment"># o</span>
<span class="predefined">next</span>(str_iter) <span class="comment"># StopIteration Error!</span>
</pre></div>
</div>

<p>At this point, you may be wondering: what&#39;s the difference between an iterator and a generator? An iterator is a more general concept: anything in Python with an <code>__next__</code> method used to produce some next value is an iterator. Generators are iterators, but not every iterator is a generator. </p>

<h3>Enumerate</h3>

<p>Sometimes when you iterate through an array, you want access not only to the elements, but also their indices. <code>enumerate</code> exposes both to you. It works by returning a tuple with the (index, value) at each iteration.</p>
<div class="CodeRay">
  <div class="code"><pre>list = [<span class="string"><span class="delimiter">&quot;</span><span class="content">first</span><span class="delimiter">&quot;</span></span>,<span class="string"><span class="delimiter">&quot;</span><span class="content">second</span><span class="delimiter">&quot;</span></span>,<span class="string"><span class="delimiter">&quot;</span><span class="content">third</span><span class="delimiter">&quot;</span></span>]

<span class="comment"># How do we get the indices at each iteration? Enumerate!</span>

<span class="keyword">for</span> idx, value <span class="keyword">in</span> <span class="predefined">enumerate</span>(<span class="predefined">list</span>):
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">index is {} and value is {}</span><span class="delimiter">&quot;</span></span>.format(idx,value))

<span class="comment"># index is 0 and value is first</span>
<span class="comment"># index is 1 and value is second</span>
<span class="comment"># index is 2 and value is third</span>
</pre></div>
</div>

<h3>all and any</h3>

<p>These are both built in functions that all us to check for a boolean matching in an iterable. </p>

<p><strong>all</strong> - returns true if <strong>all</strong> elements are truthy</p>
<div class="CodeRay">
  <div class="code"><pre><span class="predefined">all</span>([<span class="integer">0</span>]) <span class="comment"># False</span>
<span class="predefined">all</span>([<span class="integer">0</span>,<span class="integer">1</span>]) <span class="comment"># False</span>
<span class="predefined">all</span>([<span class="integer">0</span>, <span class="string"><span class="delimiter">&quot;</span><span class="delimiter">&quot;</span></span>, [<span class="integer">1</span>]]) <span class="comment"># False</span>
<span class="predefined">all</span>([<span class="integer">1</span>, <span class="string"><span class="delimiter">&quot;</span><span class="content">a</span><span class="delimiter">&quot;</span></span>, [<span class="integer">1</span>]]) <span class="comment"># True</span>
</pre></div>
</div>

<p><strong>any</strong> - returns true if <strong>any</strong> elements are truthy</p>
<div class="CodeRay">
  <div class="code"><pre><span class="predefined">any</span>([<span class="integer">0</span>]) <span class="comment"># False</span>
<span class="predefined">any</span>([<span class="integer">0</span>,<span class="integer">1</span>]) <span class="comment"># True</span>
<span class="predefined">any</span>([<span class="integer">0</span>, <span class="string"><span class="delimiter">&quot;</span><span class="delimiter">&quot;</span></span>, [<span class="integer">1</span>]]) <span class="comment"># True</span>
</pre></div>
</div>

<h3>Further Reading: Itertools</h3>

<p>To use some more advanced iterators, you can use the <code>itertools</code> module, which you can learn more about <a target="_blank" href="http://www.diveintopython3.net/advanced-iterators.html">here</a>.</p>

When you're ready, move on to Decorators.

<h1> Decorators</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Understand what a decorator is </li>
<li>Create your own decorators to add additional functionality to functions</li>
</ul>

<h3>Decorators</h3>

<p>Decorators are functions that &quot;decorate,&quot; or enhance, other functions. In order to see what this means, let&#39;s first review how we can pass functions to other functions. Remember, everything in Python is an object and objects are first class!</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">shout</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">WHOA!</span><span class="delimiter">&quot;</span></span>

<span class="keyword">def</span> <span class="function">whisper</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">Shhhh</span><span class="delimiter">&quot;</span></span>

<span class="keyword">def</span> <span class="function">perform_action</span>(func):
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">something is happening</span><span class="delimiter">&quot;</span></span>)
    <span class="keyword">return</span> func()

perform_action(shout)
<span class="comment"># something is happening</span>
<span class="comment"># 'WHOA!'</span>

perform_action(whisper)
<span class="comment"># something is happening</span>
<span class="comment"># 'Shhhh'</span>
</pre></div>
</div>

<p>We can write the behavior of a decorator like this:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">new_decorator</span>(func):
    <span class="keyword">def</span> <span class="function">wrap_func</span>():
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">code before func!</span><span class="delimiter">&quot;</span></span>)
        func()
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">code after func!</span><span class="delimiter">&quot;</span></span>)
    <span class="keyword">return</span> wrap_func

<span class="keyword">def</span> <span class="function">decorate_me</span>():
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">decorate me!</span><span class="delimiter">&quot;</span></span>)

decorate_me = new_decorator(decorate_me)

decorate_me() <span class="comment"># What do you think this will print?</span>
</pre></div>
</div>

<p>Let&#39;s now use the decorator syntax to do the same thing! When you use a decorator, the function being used to decorate is prefixed with an <code>@</code> symbol. The function you&#39;re decorating is then defined below. Take a look:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">new_decorator</span>(func):
    <span class="keyword">def</span> <span class="function">wrap_func</span>():
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">code before func!</span><span class="delimiter">&quot;</span></span>)
        func()
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">code after func!</span><span class="delimiter">&quot;</span></span>)
    <span class="keyword">return</span> wrap_func

<span class="decorator">@new_decorator</span>
<span class="keyword">def</span> <span class="function">decorate_me</span>():
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">decorate me!</span><span class="delimiter">&quot;</span></span>)
</pre></div>
</div>

<p>Note how the code inside of the <code>new_decorator</code> function decorates, or enhances, the code inside of the <code>decorate_me</code> function.</p>

<p>Let&#39;s revisit the first example but refactor it to use decorator syntax.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">perform_action</span>(func):
    <span class="keyword">def</span> <span class="function">wrap_func</span>():
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">something is happening</span><span class="delimiter">&quot;</span></span>)
        <span class="keyword">return</span> func()
    <span class="keyword">return</span> wrap_func

<span class="decorator">@perform_action</span>
<span class="keyword">def</span> <span class="function">whisper</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">Shhhh</span><span class="delimiter">&quot;</span></span>

<span class="decorator">@perform_action</span>
<span class="keyword">def</span> <span class="function">shout</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">WHOA!</span><span class="delimiter">&quot;</span></span>

whisper()
<span class="comment"># something is happening</span>
<span class="comment"># 'Shhhh'</span>

shout()
<span class="comment"># something is happening</span>
<span class="comment"># 'WHOA!'</span>
</pre></div>
</div>

<p>This code will work just fine, but if we examine the <code>__name__</code> or <code>__doc__</code> attribute for our function it will not be correct! </p>
<div class="CodeRay">
  <div class="code"><pre>shout.__name__ <span class="comment"># 'wrap_func' - oops!</span>
</pre></div>
</div>

<p>We can manually fix this, or we can use the wraps decorator from the functools module.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">functools</span> <span class="keyword">import</span> <span class="include">wraps</span> 

<span class="keyword">def</span> <span class="function">perform_action</span>(func):
    <span class="decorator">@wraps</span>(func)
    <span class="keyword">def</span> <span class="function">wrap_func</span>():
        print(<span class="string"><span class="delimiter">&quot;</span><span class="content">something is happening</span><span class="delimiter">&quot;</span></span>)
        <span class="keyword">return</span> func()
    <span class="keyword">return</span> wrap_func

<span class="decorator">@perform_action</span>
<span class="keyword">def</span> <span class="function">whisper</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">Shhhh</span><span class="delimiter">&quot;</span></span>

<span class="decorator">@perform_action</span>
<span class="keyword">def</span> <span class="function">shout</span>():
    <span class="keyword">return</span> <span class="string"><span class="delimiter">&quot;</span><span class="content">WHOA!</span><span class="delimiter">&quot;</span></span>

shout.__name__ <span class="comment"># 'shout' - much better   </span>
</pre></div>
</div>

When you're ready, move on to Lambdas and Dates
<h1>Lambdas and Dates </h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Create and use <code>lambdas</code></li>
<li>Manipulate dates and times using the <code>datetime</code> module</li>
</ul>

<h3>Lambdas</h3>

<p>The closest we have to &quot;anonymous&quot; functions in Python is lambdas. Lambdas are useful if you want to write a function which can be described in a single line of code. Here are some examples:</p>
<div class="CodeRay">
  <div class="code"><pre>add = <span class="keyword">lambda</span> x,y: x + y
double = <span class="keyword">lambda</span> val: <span class="integer">2</span> * val
yell = <span class="keyword">lambda</span> <span class="predefined">str</span>: <span class="predefined">str</span>.upper() + <span class="string"><span class="delimiter">&quot;</span><span class="content">!!!</span><span class="delimiter">&quot;</span></span>

add(<span class="integer">1</span>,<span class="integer">2</span>) <span class="comment"># 3</span>
double(<span class="integer">5</span>) <span class="comment"># 10</span>
yell(<span class="string"><span class="delimiter">&quot;</span><span class="content">hello</span><span class="delimiter">&quot;</span></span>) <span class="comment"># 'HELLO!!!'</span>

add.__name__ <span class="comment"># '&lt;lambda&gt;' </span>
add.__name__ == double.__name__ <span class="comment"># True</span>
</pre></div>
</div>

<p>Lambda functions start with the keyword <code>lambda</code>. Next comes a comma separated list of arguments, then a colon, then the expression you want the lambda to return. For simple one-line functions, lambdas can be a convenient shorthand for the traditional function definition. But these functions are anonymous; as you can see, they all share the same name. </p>

<p>One use case for lambdas is when you want to apply <code>map</code>, <code>filter</code>, or <code>reduce</code> (which as of Python 3 is part of the <code>functools</code> module). Here are some examples:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">from</span> <span class="include">functools</span> <span class="keyword">import</span> <span class="include">reduce</span>
a = [<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>,<span class="integer">5</span>]

<span class="predefined">reduce</span>(<span class="keyword">lambda</span> x,y:x+y, a) <span class="comment"># 15</span>

<span class="predefined">list</span>(<span class="predefined">map</span>(<span class="keyword">lambda</span> x:x*<span class="integer">2</span>, a)) <span class="comment"># [2,4,6,8,10]</span>
<span class="predefined">list</span>(<span class="predefined">filter</span>(<span class="keyword">lambda</span> x:x*<span class="integer">2</span> &gt; <span class="integer">5</span>, a)) <span class="comment"># [3,4]</span>
</pre></div>
</div>

<h3>Dates + Times using the Datetime class</h3>

<p>There is a quite a bit of functionality we have around dates and times with Python, but for now we&#39;ll stick to a few simple examples. Make sure you import the <code>datetime</code> module.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">datetime</span>

<span class="comment"># times</span>
<span class="comment"># hour, minute, second</span>
t = datetime.time(<span class="integer">1</span>, <span class="integer">25</span>, <span class="integer">10</span>)
t.hour <span class="comment"># 1</span>
t.microsecond <span class="comment"># 0 </span>

datetime.time.min <span class="comment"># 00:00:00</span>

today = datetime.date.today()
today.timetuple() <span class="comment">#namedtuple with data about date</span>
today.day
</pre></div>
</div>

When you're ready, move on to Generators, Iterators and Decorators Exercises

<h1>Generators, Iterators and Decorators Exercises</h1>

<p>Implement the following functions:</p>

<h3><code>get_next_multiple</code></h3>

<p>This function should accept a number and return the next number that is divisible by it.</p>
<div class="CodeRay">
  <div class="code"><pre>gen_multiple_of_two = get_next_multiple(<span class="integer">2</span>)
<span class="predefined">next</span>(gen_multiple_of_two) <span class="comment"># 2</span>
<span class="predefined">next</span>(gen_multiple_of_two) <span class="comment"># 4</span>
<span class="predefined">next</span>(gen_multiple_of_two) <span class="comment"># 6</span>
<span class="predefined">next</span>(gen_multiple_of_two) <span class="comment"># 8</span>

gen_multiple_of_thirteen = get_next_multiple(<span class="integer">13</span>)

<span class="predefined">next</span>(gen_multiple_of_thirteen) <span class="comment"># 13</span>
<span class="predefined">next</span>(gen_multiple_of_thirteen) <span class="comment"># 26</span>
<span class="predefined">next</span>(gen_multiple_of_thirteen) <span class="comment"># 39</span>
<span class="predefined">next</span>(gen_multiple_of_thirteen) <span class="comment"># 52</span>
</pre></div>
</div>

<h3><code>is_prime</code></h3>

<p>This function should accept a number and return True or False if the number is a prime number. </p>
<div class="CodeRay">
  <div class="code"><pre>is_prime(<span class="integer">11</span>) <span class="comment"># True</span>
is_prime(<span class="integer">122</span>) <span class="comment"># False</span>
</pre></div>
</div>

<h3><code>get_next_prime</code></h3>

<p>This function should return a generator that yields in the next prime number. The highest it should go should be 1000.</p>
<div class="CodeRay">
  <div class="code"><pre>gen = get_next_prime()

<span class="predefined">next</span>(gen)
</pre></div>
</div>

<h3><code>double_result</code></h3>

<p>This decorator function should return the result of another function multiplied by two</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a+b

add(<span class="integer">5</span>,<span class="integer">5</span>) <span class="comment"># 10</span>

<span class="decorator">@double_result</span>
<span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a+b

add(<span class="integer">5</span>,<span class="integer">5</span>) <span class="comment"># 20</span>
</pre></div>
</div>

<h3><code>only_even_parameters</code></h3>

<p>This decorator function should only allow a function to have even parameters or else return the string &quot;Please only use even numbers!&quot;</p>
<div class="CodeRay">
  <div class="code"><pre><span class="decorator">@only_even_parameters</span>
<span class="keyword">def</span> <span class="function">add</span>(a,b):
    <span class="keyword">return</span> a+b

add(<span class="integer">5</span>,<span class="integer">5</span>) <span class="comment"># &quot;Please add even numbers!&quot;</span>
add(<span class="integer">4</span>,<span class="integer">4</span>) <span class="comment"># 8</span>

<span class="decorator">@only_even_parameters</span>
<span class="keyword">def</span> <span class="function">multiply</span>(a,b,c,d,e):
    <span class="keyword">return</span> a*b*c*d*e
</pre></div>
</div>

<h3><code>sum_index</code></h3>

<p>This function should accept a list or tuple and return the sum of each index. As a bonus, make this function able to accept a variable number of arguments.</p>
<div class="CodeRay">
  <div class="code"><pre>sum_index([<span class="integer">1</span>,<span class="integer">2</span>,<span class="integer">3</span>,<span class="integer">4</span>]) <span class="comment"># 6</span>
</pre></div>
</div>

<h3><code>zip</code></h3>

<p>Research the built in <code>zip</code> method, what does it do? Start <a target="_blank" href="http://pavdmyt.com/python-zip-fu/">here</a></p>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_2_solutions/blob/master/generators_iterators_and_decorators/solutions.py">here</a>.</p>

When you're ready, move on to Web Scraping

<h1> Web Scraping </h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Understand what web scraping is useful for</li>
<li>Describe why <code>robots.txt</code> is important when scraping</li>
<li>Use <code>BeautifulSoup</code> to scrape web sites</li>
</ul>

<h3>Web Scraping</h3>

<p>Web scraping is the process of downloading and extracting data from a website.  There are 3 main steps in scraping:</p>

<ol>
<li>Downloading the HTML document from a website</li>
<li>Extracting data from the downloaded HTML</li>
<li>Doing something with the data (usually saving it somehow)</li>
</ol>

<p>Typically, you would want to access the data using a website&#39;s API, but often websites don&#39;t provide this programmatic access. When a website doesn&#39;t provide a programmatic way to download data (like an API) web scraping is a great way to solve the problem!</p>

<h3>Robots.txt</h3>

<p>Before you begin web scraping, it is a best practice to understand and honor the <code>robots.txt</code> file.  The file may exist on any website that you visit and its role is to tell programs (like our web scraper) about rules on what it should and should not download on the site.  Here is Rithm School&#39;s <a target="_blank" href="https://www.rithmschool.com/robots.txt">robots.txt</a> file.  As you can see, it doesn&#39;t provide any restrictions.  Compare that file to Craigslist&#39;s <a target="_blank" href="http://craigslist.org/robots.txt">robots.txt</a> file which is much more restrictive on what can be downloaded by a program.</p>

<p>You can find out more information about the robots.txt file at <a target="_blank" href="http://www.robotstxt.org/robotstxt.html">http://www.robotstxt.org/robotstxt.html</a></p>

<h3>Beautiful Soup</h3>

<p>The library we will be using for web scraping is called <code>BeautifulSoup</code>, which you can install using <code>pip3 install beautifulsoup4</code>.  You can read more about it <a target="_blank" href="https://www.crummy.com/software/BeautifulSoup/bs4/doc/#quick-start">here</a>.</p>

<p>Keeping in mind that there are 3 steps to web scraping, <code>BeautifulSoup</code> is a tool that helps with the second step, extracting data from the downloaded HTML.  Without a tool like <code>BeautifulSoup</code> the job of extracting data out of HTML is a very hard problem.</p>

<p>Here is an example of <code>BeautifulSoup</code> in action.  The code uses <code>find_all</code> and <code>text</code> to access the names in the li elements:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">bs4</span>
html = <span class="string"><span class="delimiter">&quot;&quot;&quot;</span><span class="content">
</span><span class="content">&lt;html&gt;</span><span class="content">
</span><span class="content">&lt;body&gt;</span><span class="content">
</span><span class="content">  &lt;h3&gt;Names&lt;/h3&gt;</span><span class="content">
</span><span class="content">  &lt;ul&gt;</span><span class="content">
</span><span class="content">    &lt;li&gt;Tim&lt;/li&gt;</span><span class="content">
</span><span class="content">    &lt;li&gt;Matt&lt;/li&gt;</span><span class="content">
</span><span class="content">    &lt;li&gt;Elie&lt;/li&gt;</span><span class="content">
</span><span class="content">    &lt;li&gt;Janey&lt;/li&gt;</span><span class="content">
</span><span class="content">  &lt;/ul&gt;</span><span class="content">
</span><span class="content">&lt;/body&gt;</span><span class="content">
</span><span class="content">&lt;/html&gt;</span><span class="content">
</span><span class="delimiter">&quot;&quot;&quot;</span></span>

soup = bs4.BeautifulSoup(html, <span class="string"><span class="delimiter">&quot;</span><span class="content">html.parser</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">for</span> li <span class="keyword">in</span> soup.find_all(<span class="string"><span class="delimiter">'</span><span class="content">li</span><span class="delimiter">'</span></span>):
    print(li.text)

</pre></div>
</div>

<p>Notice that we&#39;re using <code>BeautifulSoup</code> and passing it two parameters: the html is the first and the type of parser is the second.  For our purposes, the <code>html.parser</code> will work well.</p>

<p>Next, let&#39;s use <code>BeautifulSoup</code> to find an element by id:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">bs4</span>
html = <span class="string"><span class="delimiter">&quot;&quot;&quot;</span><span class="content">
</span><span class="content">&lt;html&gt;</span><span class="content">
</span><span class="content">&lt;body&gt;</span><span class="content">
</span><span class="content">  &lt;div id=&quot;interesting-data&quot;&gt;Moxie is my cat&lt;/div&gt;</span><span class="content">
</span><span class="content">&lt;/body&gt;</span><span class="content">
</span><span class="content">&lt;/html&gt;</span><span class="content">
</span><span class="delimiter">&quot;&quot;&quot;</span></span>

soup = bs4.BeautifulSoup(html, <span class="string"><span class="delimiter">&quot;</span><span class="content">html.parser</span><span class="delimiter">&quot;</span></span>)

div = soup.find(id=<span class="string"><span class="delimiter">&quot;</span><span class="content">interesting-data</span><span class="delimiter">&quot;</span></span>)
print(div.text)
</pre></div>
</div>

<p>Here are some other useful elements that you can take advantage of in <code>BeautifulSoup</code>:</p>

<p><code>.select()</code> - find an element / elements using CSS selectors.</p>

<p><code>.children</code> - find all children of an element</p>

<p><code>.parent</code> - find the parent element of a specific element</p>

<h3>Downloading And Scraping a Page</h3>

<p>Now that we&#39;re familiar with <code>BeautifulSoup</code>, we are going to download real html from a site and scrape some data!</p>

<p>Create a file called <code>first_scraping.py</code> and add the following (make sure you <code>pip3 install beautifulsoup4</code> first).</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">urllib.request</span>
<span class="keyword">import</span> <span class="include">bs4</span>

url = <span class="string"><span class="delimiter">'</span><span class="content">https://news.ycombinator.com/</span><span class="delimiter">'</span></span>
data = urllib.request.urlopen(url).read()
soup = bs4.BeautifulSoup(data, <span class="string"><span class="delimiter">&quot;</span><span class="content">html.parser</span><span class="delimiter">&quot;</span></span>)

links = soup.select(<span class="string"><span class="delimiter">&quot;</span><span class="content">a.storylink</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">for</span> link <span class="keyword">in</span> links:
    print(<span class="string"><span class="delimiter">&quot;</span><span class="content">{} {}</span><span class="delimiter">&quot;</span></span>.format(link[<span class="string"><span class="delimiter">'</span><span class="content">href</span><span class="delimiter">'</span></span>],link.text))
</pre></div>
</div>

<p>Now run <code>python3 first_scraping.py</code> and examine the data you scraped!</p>

<h3>Saving Scraped Data To CSV</h3>

<p>Let&#39;s modify the previous example and save our results to a TSV file (We chose TSV, tab separated values, because the article titles often have commas in them):</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">urllib.request</span>
<span class="keyword">import</span> <span class="include">bs4</span>
<span class="keyword">import</span> <span class="include">csv</span>

url = <span class="string"><span class="delimiter">'</span><span class="content">https://news.ycombinator.com/</span><span class="delimiter">'</span></span>
data = urllib.request.urlopen(url).read()
soup = bs4.BeautifulSoup(data, <span class="string"><span class="delimiter">&quot;</span><span class="content">html.parser</span><span class="delimiter">&quot;</span></span>)

links = soup.select(<span class="string"><span class="delimiter">&quot;</span><span class="content">a.storylink</span><span class="delimiter">&quot;</span></span>)

<span class="keyword">with</span> <span class="predefined">open</span>(<span class="string"><span class="delimiter">'</span><span class="content">articles.tsv</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">w</span><span class="delimiter">'</span></span>) <span class="keyword">as</span> tsvfile:
    writer = csv.writer(tsvfile, delimiter=<span class="string"><span class="delimiter">&quot;</span><span class="char">\t</span><span class="delimiter">&quot;</span></span>)
    writer.writerow( (<span class="string"><span class="delimiter">'</span><span class="content">Link</span><span class="delimiter">'</span></span>, <span class="string"><span class="delimiter">'</span><span class="content">Title</span><span class="delimiter">'</span></span>) )
    <span class="keyword">for</span> link <span class="keyword">in</span> links:
        writer.writerow( (link[<span class="string"><span class="delimiter">'</span><span class="content">href</span><span class="delimiter">'</span></span>], link.text) )

</pre></div>
</div>

<p>Great! Now you&#39;ve done all 3 steps of scaping: downloading, extracting and saving!</p>

When you're ready, move on to Server Side HTTP Requests

<h1>Server Side HTTP Requests</h1>

<h3>Objectives</h3>

<p>By the end of this chapter, you should be able to:</p>

<ul>
<li>Use the <code>requests</code> module to perform server side requests</li>
<li>Compare and contrast client and server side API requests</li>
</ul>

<h3>Requests</h3>

<p>In this section, we will be using terms like HTTP, APIs, AJAX and headers. If you are not familiar with these terms, take a look at the section on How The Web Works in our Intermediate JavaScript Part II course. </p>

<p>Using Python, we can make make HTTP requests to send and retrieve data from APIs. Although we can do this with JavaScript as well (using a technology called AJAX), using JavaScript will not always work because of security reasons. </p>

<p>Instead, we can make requests from one server to another server (and if you are comfortable with JavaScript, you can send back a response to the browser from &quot;our&quot; server). Here is what that might look like.</p>

<p>To issue server side requests we use the <code>requests</code> module, which you can install using <code>pip3 install requests</code>. You can read more about it <a target="_blank" href="http://docs.python-requests.org/en/master/">here</a>.</p>

<p>Let&#39;s start with a very simple example to get data from the OMDB API.</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">requests</span>

<span class="comment"># Make an HTTP GET request to a specific URL</span>
r = requests.get(<span class="string"><span class="delimiter">'</span><span class="content">http://omdbapi.com?t=titanic</span><span class="delimiter">'</span></span>) <span class="comment"># returns a response object</span>
r.status_code <span class="comment"># 200</span>
r.ok <span class="comment"># True</span>
r.headers <span class="comment"># see a dictionary of HTTP headers</span>
r.json() <span class="comment"># Examine what this data looks like in JSON</span>
</pre></div>
</div>

<p>We can also use the requests module to make a POST request:</p>
<div class="CodeRay">
  <div class="code"><pre><span class="keyword">import</span> <span class="include">requests</span>

payload = <span class="predefined">dict</span>(id=<span class="integer">1</span>)

r = requests.post(<span class="string"><span class="delimiter">'</span><span class="content">some_url</span><span class="delimiter">'</span></span>, params=payload)

r.text <span class="comment"># see your params in an args dictionary</span>
</pre></div>
</div>

<p>The requests module is very useful for sending and retrieving data from an API and can also be used to authenticate users (logging in through Facebook / Twitter / etc.).</p>

When you're ready, move on to Web Scraping Exercises

<h1>Web Scraping Exercises</h1>
<h3>Part 1 - Web Scraping</h3>

<p>Write a Python program that uses BeautifulSoup to go to <code>https://news.google.com</code> and prints out all of the headlines on the page. Then, write a function called <code>find_headline_by_keyword</code> which lets you search through those headlines for keywords, and returns to you a list of all of the headlines that match all the keywords you provide.</p>

<h3>Part 2 - Web Scraping + File IO</h3>

<p><a target="_blank" href="https://en.wikipedia.org/wiki/United_States_presidential_election">This</a> Wikipedia page has a table with data on all of the US Presidential elections. Our goal is to use Beautiful Soup to scrape some of this data into a CSV file. The columns of the CSV should be: order, year, winner, winner electoral votes, runner-up, and runner-up electoral votes. Use commas as the delimiter. For instance, after the header row, the first row of data should look like this:</p>
<div class="CodeRay">
  <div class="code"><pre>1st,1788–1789,George Washington,69,John Adams,34
</pre></div>
</div>

<p>(Hint: use the <code>pdb</code> debugger! Setting break points is a great way to experiment with your code to make sure that you&#39;re selecting the right elements and correctly targeting the text that you&#39;re interested in.)</p>

<h3>Part 3 - Server Side Requests</h3>

<p>Using the <code>requests</code> module and the <a target="_blank" href="https://www.omdbapi.com/">OMDB API</a>, build an application that prompts the user for two pieces of information, the name of an actor/actress and a movie. Your program should tell the user if that actor or actress was in that movie (this will only work for leading actors and actresses). As a bonus, add functionality to tell users who the director and writer of a movie were.</p>

<p>For solutions to these exercises, click <a target="_blank" href="https://github.com/rithmschool/python_fundamentals_part_2_solutions/blob/master/web_scraping_and_server_side_requests/part_3_solution.py">here</a>.</p>
