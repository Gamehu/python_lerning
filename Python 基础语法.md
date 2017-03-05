<div class="article-body">
		
			<div class="article-intro" id="content">
			
			<h1>Python <span class="color_h1">基础语法</span></h1>

<p>Python语言与Perl，C和Java等语言有许多相似之处。但是，也存在一些差异。</p>
<p>在本章中我们将来学习Python的基础语法，让你快速学会Python编程。</p>


<hr><h2>第一个Python程序</h2>
<h3>交互式编程</h3>
<p>交互式编程不需要创建脚本文件，是通过 Python 解释器的交互模式进来编写代码。</p><p>
linux上你只需要在命令行中输入 Python 命令即可启动交互式编程,提示窗口如下：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ python
</span><span class="typ">Python</span><span class="pln"> </span><span class="lit">2.7</span><span class="pun">.</span><span class="lit">6</span><span class="pln"> </span><span class="pun">(</span><span class="kwd">default</span><span class="pun">,</span><span class="pln"> </span><span class="typ">Sep</span><span class="pln">  </span><span class="lit">9</span><span class="pln"> </span><span class="lit">2014</span><span class="pun">,</span><span class="pln"> </span><span class="lit">15</span><span class="pun">:</span><span class="lit">04</span><span class="pun">:</span><span class="lit">36</span><span class="pun">)</span><span class="pln"> 
</span><span class="pun">[</span><span class="pln">GCC </span><span class="lit">4.2</span><span class="pun">.</span><span class="lit">1</span><span class="pln"> </span><span class="typ">Compatible</span><span class="pln"> </span><span class="typ">Apple</span><span class="pln"> LLVM </span><span class="lit">6.0</span><span class="pln"> </span><span class="pun">(</span><span class="pln">clang</span><span class="pun">-</span><span class="lit">600.0</span><span class="pun">.</span><span class="lit">39</span><span class="pun">)]</span><span class="pln"> on darwin
</span><span class="typ">Type</span><span class="pln"> </span><span class="str">"help"</span><span class="pun">,</span><span class="pln"> </span><span class="str">"copyright"</span><span class="pun">,</span><span class="pln"> </span><span class="str">"credits"</span><span class="pln"> </span><span class="kwd">or</span><span class="pln"> </span><span class="str">"license"</span><span class="pln"> </span><span class="kwd">for</span><span class="pln"> more information</span><span class="pun">.</span><span class="pln">
</span><span class="pun">&gt;&gt;&gt;</span><span class="pln"> </span></pre>
<p>
Window上在安装Python时已经已经安装了默认的交互式编程客户端，提示窗口如下：</p>
<p><img src="http://www.runoob.com/wp-content/uploads/2013/11/python-shell.jpg" alt="python-shell" class="alignnone size-full wp-image-7710" srcset="http://www.runoob.com/wp-content/uploads/2013/11/python-shell.jpg 678w, http://www.runoob.com/wp-content/uploads/2013/11/python-shell-300x120.jpg 300w" sizes="(max-width: 678px) 100vw, 678px" height="273" width="678"></p>
<p>在 python 提示符中输入以下文本信息，然后按 Enter 键查看运行效果：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pun">&gt;&gt;&gt;</span><span class="pln"> </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"Hello, Python!"</span><span class="pun">;</span></pre>
<p>在 Python  2.7.6 版本中,以上实例输出结果如下：</p>
<pre class="prettyprint prettyprinted" style=""><span class="typ">Hello</span><span class="pun">,</span><span class="pln"> </span><span class="typ">Python</span><span class="pun">!</span></pre>
<h3>脚本式编程</h3>
<p>通过脚本参数调用解释器开始执行脚本，直到脚本执行完毕。当脚本执行完成后，解释器不再有效。</p>

<p>让我们写一个简单的Python脚本程序。所有Python文件将以.py为扩展名。将以下的源代码拷贝至test.py文件中。</p>
<pre class="prettyprint prettyprinted" style=""><span class="kwd">print</span><span class="pln"> </span><span class="str">"Hello, Python!"</span><span class="pun">;</span></pre>
<p>这里，假设你已经设置了Python解释器PATH变量。使用以下命令运行程序：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ python test</span><span class="pun">.</span><span class="pln">py</span></pre>
<p>输出结果：</p>
<pre class="prettyprint prettyprinted" style=""><span class="typ">Hello</span><span class="pun">,</span><span class="pln"> </span><span class="typ">Python</span><span class="pun">!</span></pre>
<p>让我们尝试另一种方式来执行Python脚本。修改test.py文件，如下所示：</p>
<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">

</span><span class="kwd">print</span><span class="pln"> </span><span class="str">"Hello, Python!"</span><span class="pun">;</span></pre>
<p>这里，假定您的Python解释器在/usr/bin目录中，使用以下命令执行脚本：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ chmod </span><span class="pun">+</span><span class="pln">x test</span><span class="pun">.</span><span class="pln">py     </span><span class="com"># 脚本文件添加可执行权限</span><span class="pln">
$ </span><span class="pun">./</span><span class="pln">test</span><span class="pun">.</span><span class="pln">py</span></pre>
<p>输出结果：</p>
<pre class="prettyprint prettyprinted" style=""><span class="typ">Hello</span><span class="pun">,</span><span class="pln"> </span><span class="typ">Python</span><span class="pun">!</span></pre>
<hr><h2>Python 标识符</h2>
<p>在python里，标识符有字母、数字、下划线组成。</p>
<p>在python中，所有标识符可以包括英文、数字以及下划线（_），但不能以数字开头。</p>
<p>python中的标识符是区分大小写的。</p>
<p>以下划线开头的标识符是有特殊意义的。以单下划线开头（_foo）的代表不能直接访问的类属性，需通过类提供的接口进行访问，不能用"from xxx import *"而导入；</p>
<p>以双下划线开头的（__foo）代表类的私有成员；以双下划线开头和结尾的（__foo__）代表python里特殊方法专用的标识，如__init__（）代表类的构造函数。</p>

<hr><h2>Python保留字符</h2>
<p>下面的列表显示了在Python中的保留字。这些保留字不能用作常数或变数，或任何其他标识符名称。</p>
<p>所有Python的关键字只包含小写字母。</p>
<table class="reference">
<tbody><tr><td>and</td><td>exec</td><td>not</td></tr>
<tr><td>assert</td><td>finally</td><td>or</td></tr>
<tr><td>break</td><td>for</td><td>pass</td></tr>
<tr><td>class</td><td>from</td><td>print</td></tr>
<tr><td>continue</td><td>global</td><td>raise</td></tr>
<tr><td>def</td><td>if</td><td>return</td></tr>
<tr><td>del</td><td>import</td><td>try</td></tr>
<tr><td>elif</td><td>in</td><td>while</td></tr>
<tr><td>else</td><td>is</td><td>with </td></tr>
<tr><td>except</td><td>lambda</td><td>yield</td></tr>
</tbody></table>
<hr><h2>行和缩进</h2>
<p>学习Python与其他语言最大的区别就是，Python的代码块不使用大括号（{}）来控制类，函数以及其他逻辑判断。python最具特色的就是用缩进来写模块。</p>
<p>缩进的空白数量是可变的，但是所有代码块语句必须包含相同的缩进空白数量，这个必须严格执行。如下所示：</p>
<pre class="prettyprint prettyprinted" style=""><span class="kwd">if</span><span class="pln"> </span><span class="kwd">True</span><span class="pun">:</span><span class="pln">
    </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"True"</span><span class="pln">
</span><span class="kwd">else</span><span class="pun">:</span><span class="pln">
  </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"False"</span><span class="pln">
 </span></pre>
<p>以下代码将会执行错误：</p>
<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">
</span><span class="com"># -*- coding: UTF-8 -*-</span><span class="pln">
</span><span class="com"># 文件名：test.py</span><span class="pln">

 </span><span class="kwd">if</span><span class="pln"> </span><span class="kwd">True</span><span class="pun">:</span><span class="pln">
    </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"Answer"</span><span class="pln">
    </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"True"</span><span class="pln">
</span><span class="kwd">else</span><span class="pun">:</span><span class="pln">
    </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"Answer"</span><span class="pln">
    </span><span class="com"># 没有严格缩进，在执行时会报错</span><span class="pln">
  </span><span class="kwd">print</span><span class="pln"> </span><span class="str">"False"</span></pre>
<p> 执行以上代码，会出现如下错误提醒：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ python test</span><span class="pun">.</span><span class="pln">py  
  </span><span class="typ">File</span><span class="pln"> </span><span class="str">"test.py"</span><span class="pun">,</span><span class="pln"> line </span><span class="lit">5</span><span class="pln">
    </span><span class="kwd">if</span><span class="pln"> </span><span class="kwd">True</span><span class="pun">:</span><span class="pln">
    </span><span class="pun">^</span><span class="pln">
</span><span class="typ">IndentationError</span><span class="pun">:</span><span class="pln"> unexpected indent</span></pre>
<p><b>IndentationError: unexpected indent</b> 错误是python编译器是在告诉你"Hi，老兄，你的文件里格式不对了，可能是tab和空格没对齐的问题"，所有python对格式要求非常严格。</p>

<p>如果是 <b>IndentationError: unindent does not match any outer indentation level</b>错误表明，你使用的缩进方式不一致，有的是 tab 键缩进，有的是空格缩进，改为一致即可。</p>
<p>因此，在Python的代码块中必须使用相同数目的行首缩进空格数。</p>
<p>建议你在每个缩进层次使用 <strong>单个制表符</strong> 或 <strong>两个空格</strong> 或 <strong>四个空格</strong> , 切记不能混用</p>
<hr><h2>多行语句</h2>
<p>Python语句中一般以新行作为为语句的结束符。</p>
<p>但是我们可以使用斜杠（ \）将一行的语句分为多行显示，如下所示：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">total </span><span class="pun">=</span><span class="pln"> item_one </span><span class="pun">+</span><span class="pln"> \
        item_two </span><span class="pun">+</span><span class="pln"> \
        item_three</span></pre>
<p>语句中包含[], {} 或 () 括号就不需要使用多行连接符。如下实例：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">days </span><span class="pun">=</span><span class="pln"> </span><span class="pun">[</span><span class="str">'Monday'</span><span class="pun">,</span><span class="pln"> </span><span class="str">'Tuesday'</span><span class="pun">,</span><span class="pln"> </span><span class="str">'Wednesday'</span><span class="pun">,</span><span class="pln">
        </span><span class="str">'Thursday'</span><span class="pun">,</span><span class="pln"> </span><span class="str">'Friday'</span><span class="pun">]</span></pre>
<hr><h2>Python 引号</h2>
<p>Python 可以使用引号( <strong>'</strong> )、双引号( <strong>"</strong> )、三引号( <strong>'''</strong> 或 <strong>"""</strong> ) 来表示字符串，引号的开始与结束必须的相同类型的。 </p>
<p>其中三引号可以由多行组成，编写多行文本的快捷语法，常用语文档字符串，在文件的特定地点，被当做注释。</p>

<pre class="prettyprint prettyprinted" style=""><span class="pln">word </span><span class="pun">=</span><span class="pln"> </span><span class="str">'word'</span><span class="pln">
sentence </span><span class="pun">=</span><span class="pln"> </span><span class="str">"这是一个句子。"</span><span class="pln">
paragraph </span><span class="pun">=</span><span class="pln"> </span><span class="str">"""这是一个段落。
包含了多个语句"""</span></pre>

<hr><h2>Python注释</h2>
<p>python中单行注释采用 # 开头。</p>

<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">
</span><span class="com"># -*- coding: UTF-8 -*-</span><span class="pln">
</span><span class="com"># 文件名：test.py</span><span class="pln">

</span><span class="com"># 第一个注释</span><span class="pln">
</span><span class="kwd">print</span><span class="pln"> </span><span class="str">"Hello, Python!"</span><span class="pun">;</span><span class="pln">  </span><span class="com"># 第二个注释</span></pre>
<p>输出结果：</p>
<pre class="prettyprint prettyprinted" style=""><span class="typ">Hello</span><span class="pun">,</span><span class="pln"> </span><span class="typ">Python</span><span class="pun">!</span></pre>
<p>注释可以在语句或表达式行末：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">name </span><span class="pun">=</span><span class="pln"> </span><span class="str">"Madisetti"</span><span class="pln"> </span><span class="com"># 这是一个注释</span></pre>
<p>python 中多行注释使用三个单引号(''')或三个双引号(""")。</p>
<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">
</span><span class="com"># -*- coding: UTF-8 -*-</span><span class="pln">
</span><span class="com"># 文件名：test.py</span><span class="pln">


</span><span class="str">'''
这是多行注释，使用单引号。
这是多行注释，使用单引号。
这是多行注释，使用单引号。
'''</span><span class="pln">

</span><span class="str">"""
这是多行注释，使用双引号。
这是多行注释，使用双引号。
这是多行注释，使用双引号。
"""</span></pre>
<hr><h2>Python空行</h2>
<p>函数之间或类的方法之间用空行分隔，表示一段新的代码的开始。类和函数入口之间也用一行空行分隔，以突出函数入口的开始。</p>
<p>空行与代码缩进不同，空行并不是Python语法的一部分。书写时不插入空行，Python解释器运行也不会出错。但是空行的作用在于分隔两段不同功能或含义的代码，便于日后代码的维护或重构。</p><p>记住：空行也是程序代码的一部分。</p>
<hr><h2>等待用户输入</h2>
<p>下面的程序在按回车键后就会等待用户输入：</p>
<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">

raw_input</span><span class="pun">(</span><span class="str">"\n\nPress the enter key to exit."</span><span class="pun">)</span></pre>
<p>以上代码中 ，"\n\n"在结果输出前会输出两个新的空行。一旦用户按下 enter(回车) 键退出，其它键显示。</p>
<hr><h2>同一行显示多条语句</h2>
Python可以在同一行中使用多条语句，语句之间使用分号(;)分割，以下是一个简单的实例：<p></p>
<pre class="prettyprint prettyprinted" style=""><span class="com">#!/usr/bin/python</span><span class="pln">

</span><span class="kwd">import</span><span class="pln"> sys</span><span class="pun">;</span><span class="pln"> x </span><span class="pun">=</span><span class="pln"> </span><span class="str">'runoob'</span><span class="pun">;</span><span class="pln"> sys</span><span class="pun">.</span><span class="pln">stdout</span><span class="pun">.</span><span class="pln">write</span><span class="pun">(</span><span class="pln">x </span><span class="pun">+</span><span class="pln"> </span><span class="str">'\n'</span><span class="pun">)</span></pre>
<p>执行以上代码，输入结果为：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ python test</span><span class="pun">.</span><span class="pln">py
runoob</span></pre>
<hr><h2>多个语句构成代码组</h2>
<p>缩进相同的一组语句构成一个代码块，我们称之代码组。</p>
<p>像if、while、def和class这样的复合语句，首行以关键字开始，以冒号( : )结束，该行之后的一行或多行代码构成代码组。</p>
<p>我们将首行及后面的代码组称为一个子句(clause)。</p>
<p>如下实例：</p>
<pre class="prettyprint prettyprinted" style=""><span class="kwd">if</span><span class="pln"> expression </span><span class="pun">:</span><span class="pln"> 
   suite 
</span><span class="kwd">elif</span><span class="pln"> expression </span><span class="pun">:</span><span class="pln">  
   suite  
</span><span class="kwd">else</span><span class="pln"> </span><span class="pun">:</span><span class="pln">  
   suite </span></pre>
<hr><h2>命令行参数</h2>
<p>很多程序可以执行一些操作来查看一些基本信，Python可以使用-h参数查看各参数帮助信息：</p>
<pre class="prettyprint prettyprinted" style=""><span class="pln">$ python </span><span class="pun">-</span><span class="pln">h 
usage</span><span class="pun">:</span><span class="pln"> python </span><span class="pun">[</span><span class="pln">option</span><span class="pun">]</span><span class="pln"> </span><span class="pun">...</span><span class="pln"> </span><span class="pun">[-</span><span class="pln">c cmd </span><span class="pun">|</span><span class="pln"> </span><span class="pun">-</span><span class="pln">m mod </span><span class="pun">|</span><span class="pln"> file </span><span class="pun">|</span><span class="pln"> </span><span class="pun">-]</span><span class="pln"> </span><span class="pun">[</span><span class="pln">arg</span><span class="pun">]</span><span class="pln"> </span><span class="pun">...</span><span class="pln"> 
</span><span class="typ">Options</span><span class="pln"> </span><span class="kwd">and</span><span class="pln"> arguments </span><span class="pun">(</span><span class="kwd">and</span><span class="pln"> corresponding environment variables</span><span class="pun">):</span><span class="pln"> 
</span><span class="pun">-</span><span class="pln">c cmd </span><span class="pun">:</span><span class="pln"> program passed </span><span class="kwd">in</span><span class="pln"> </span><span class="kwd">as</span><span class="pln"> </span><span class="kwd">string</span><span class="pln"> </span><span class="pun">(</span><span class="pln">terminates option list</span><span class="pun">)</span><span class="pln"> 
</span><span class="pun">-</span><span class="pln">d     </span><span class="pun">:</span><span class="pln"> debug output </span><span class="kwd">from</span><span class="pln"> parser </span><span class="pun">(</span><span class="pln">also PYTHONDEBUG</span><span class="pun">=</span><span class="pln">x</span><span class="pun">)</span><span class="pln"> 
</span><span class="pun">-</span><span class="pln">E     </span><span class="pun">:</span><span class="pln"> ignore environment variables </span><span class="pun">(</span><span class="pln">such </span><span class="kwd">as</span><span class="pln"> PYTHONPATH</span><span class="pun">)</span><span class="pln"> 
</span><span class="pun">-</span><span class="pln">h     </span><span class="pun">:</span><span class="pln"> </span><span class="kwd">print</span><span class="pln"> </span><span class="kwd">this</span><span class="pln"> help message </span><span class="kwd">and</span><span class="pln"> </span><span class="kwd">exit</span><span class="pln"> 
 
</span><span class="pun">[</span><span class="pln"> etc</span><span class="pun">.</span><span class="pln"> </span><span class="pun">]</span><span class="pln"> </span></pre>    
<p>我们在使用脚本形式执行 Python 时，可以接收命令行输入的参数，具体使用可以参照 <a href="python-command-line-arguments.html" target="_blank">Python 命令行参数</a>。</p>			
	
  转自			
!(http://www.runoob.com/python/python-basic-syntax.html) 
		</div>
