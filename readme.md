Welcome to my test

I got a little short on time so I couldn't test the code but it should work in theory. I didn't know we had to put part A in this readme until after I already made a table in word, so part A is a pdf labelled as "partA.pdf".
Everything else should be in "test2.ipynb"

Part B. Productions

<stmt> --> <block> | <if_stmt> | <while_loop> | <assignment>
<block> --> `{`{<stmt> `;` }`}`
<if_stmt>   -->  `maybe``(`<bool_stmt> `)`<stmt>[`probably ` <stmt>]
<do_while> --> `bing` <block> <while_loop>
<while_loop> -->  `bong``(`<bool_stmt>`)`<stmt>
<for_loop> --> `turtle``(`<bool_stmt>`)`<block>
<assignment> --> `set` <factor> `=` <expr>
<expr> --> <term> {(`+`|`-`)<term>}
<term> --> <factor>{(`*`|`/`|`%`)<factor>}
<factor> -->  `a` | `b`|`c`|`d`|`{ ` <expr> `}`




Part C. LL grammar

All the rules conform to the standard of LL Grammar. The pairwise disjointness test confirms conformity. For the rules to pass the test, the rules must not have left-hand recursion. This means that no two rules could have the same first statement because if they did, the program could go in different paths. This makes the grammar non-deterministic, thus making it ambiguous. For example, <assignment> and <factor> could both have the ‘set’ keyword in to ensure that both are variables. However, this would cause the grammar to fail the pairwise disjointness test. Since all the rules have unique keywords, the grammar passes the test. Thus conforming to the standard of LL Grammar. 

Part D. Unambigious 

The previous part effectively confirms the grammar is unambigious because there is no way for the grammar to generate a multiple paths for a program using this language.