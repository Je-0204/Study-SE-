# Study-SE-

# Tables

- Tables는 pipes( | )와 hyphens( - ) 로 나뉜다.
## Code EX_1

    <table>
    <thead>
    <tr>
    <th>foo</th>
    <th>bar</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td>baz</td>
    <td>bim</td>
    </tr>
    </tbody>
    </table>
 
이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>foo</th>
<th>bar</th>
</tr>
</thead>
<tbody>
<tr>
<td>baz</td>
<td>bim</td>
</tr>
</tbody>
</table>

## Code EX_2

    <table>
    <thead>
    <tr>
    <th align="center">abc</th>
    <th align="right">defghi</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td align="center">bar</td>
    <td align="right">baz</td>
    </tr>
    </tbody>
    </table>
  
이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th align="center">abc</th>
<th align="right">defghi</th>
</tr>
</thead>
<tbody>
<tr>
<td align="center">bar</td>
<td align="right">baz</td>
</tr>
</tbody>
</table>
  
한 열의 길이를 맞출 필요는 없습니다.  

## Code EX_3

    <table>
    <thead>
    <tr>
    <th>f|oo</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td>b <code>|</code> az</td>
    </tr>
    <tr>
    <td>b <strong>|</strong> im</td>
    </tr>
    </tbody>
    </table>
    
이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>f|oo</th>
</tr>
</thead>
<tbody>
<tr>
<td>b <code>|</code> az</td>
</tr>
<tr>
<td>b <strong>|</strong> im</td>
</tr>
</tbody>
</table>

파이프를 안에 추가할 수도 있습니다.

## Code EX_4

    <table>
    <thead>
    <tr>
    <th>abc</th>
    <th>def</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td>bar</td>
    <td>baz</td>
    </tr>
    </tbody>
    </table>
    <blockquote>
    <p>bar</p>
    </blockquote>

이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>abc</th>
<th>def</th>
</tr>
</thead>
<tbody>
<tr>
<td>bar</td>
<td>baz</td>
</tr>
</tbody>
</table>
<blockquote>
<p>bar</p>
</blockquote>

그리고 또 하나의 코드를 보면

    <table>
    <thead>
    <tr>
    <th>abc</th>
    <th>def</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td>bar</td>
    <td>baz</td>
    </tr>
    <tr>
    <td>bar</td>
    <td></td>
    </tr>
    </tbody>
    </table>
    <p>bar</p>

이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>abc</th>
<th>def</th>
</tr>
</thead>
<tbody>
<tr>
<td>bar</td>
<td>baz</td>
</tr>
<tr>
<td>bar</td>
<td></td>
</tr>
</tbody>
</table>
<p>bar</p>

이렇게 테이블이 파손된 모습을 볼 수 있습니다.

## Code EX_5

    <p>| abc | def |
    | --- |
    | bar |</p>

이 코드의 실행 결과입니다.
<p>| abc | def |
| --- |
| bar |</p>

Header row는 cell number의 delimiter row와 일치해야 합니다.

## Code EX_6

    <table>
    <thead>
    <tr>
    <th>abc</th>
    <th>def</th>
    </tr>
    </thead>
    <tbody>
    <tr>
    <td>bar</td>
    <td></td>
    </tr>
    <tr>
    <td>bar</td>
    <td>baz</td>
    </tr>
    </tbody>
    </table>
    
이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>abc</th>
<th>def</th>
</tr>
</thead>
<tbody>
<tr>
<td>bar</td>
<td></td>
</tr>
<tr>
<td>bar</td>
<td>baz</td>
</tr>
</tbody>
</table>

헤더 행에 cell number보다 적은 cell number가 있으면 빈 cell이 삽입됩니다.  
하지만 cell number보다 큰 cell number가 있으면 무시됩니다.

## Code EX_7

    <table>
    <thead>
    <tr>
    <th>abc</th>
    <th>def</th>
    </tr>
    </thead>
    </table>
    
이 코드의 실행 결과입니다.
<table>
<thead>
<tr>
<th>abc</th>
<th>def</th>
</tr>
</thead>
</table>
        
body에 행이 없는 경우 HTML 출력에 \<tbody>가 생성되지 않습니다.
  
# Task list items

## Code EX_1

    <ul>
    <li><input disabled="" type="checkbox"> foo</li>
    <li><input checked="" disabled="" type="checkbox"> bar</li>
    </ul>
    
이 코드의 실행 결과입니다.
<ul>
<li><input disabled="" type="checkbox"> foo</li>
<li><input checked="" disabled="" type="checkbox"> bar</li>
</ul>

Task List Item Marker는 [, 공백 또는 x(X), ]로 구성되어 있습니다.  
만약 []사이의 문자가 공백이면 checkbox가 unchecked될 것이고, 그렇지 않으면 checked가 될 것입니다.
## Code EX_2

    <ul>
    <li><input checked="" disabled="" type="checkbox"> foo
    <ul>
    <li><input disabled="" type="checkbox"> bar</li>
    <li><input checked="" disabled="" type="checkbox"> baz</li>
    </ul>
    </li>
    <li><input disabled="" type="checkbox"> bim</li>
    </ul>
    
이 코드의 실행 결과입니다.
<ul>
<li><input checked="" disabled="" type="checkbox"> foo
<ul>
<li><input disabled="" type="checkbox"> bar</li>
<li><input checked="" disabled="" type="checkbox"> baz</li>
</ul>
</li>
<li><input disabled="" type="checkbox"> bim</li>
</ul>

Task List Item은 중첩될 수도 있습니다.
  
# Strikethrough

## Code EX_1

    <p><del>Hi</del> Hello, world!</p>
 
이 코드의 실행 결과입니다.
<p><del>Hi</del> Hello, world!</p>

Strikethrough text는 two tildes (~)로 묶인 텍스트입니다.

## Code EX_2

    <p>This ~~has a</p>
    <p>new paragraph~~.</p>
    
이 코드의 실행 결과입니다.
<p>This ~~has a</p>
<p>new paragraph~~.</p>

# Autolinks

## Code EX_1

    <p><a href="http://www.commonmark.org">www.commonmark.org</a></p>

이 코드의 실행 결과입니다.
<p><a href="http://www.commonmark.org">www.commonmark.org</a></p>

기본적으로 이렇게 씁니다.

## Code EX_2

    <p>Visit <a href="http://www.commonmark.org/help">www.commonmark.org/help</a> for more information.</p>

이 코드의 실행 결과입니다.
<p>Visit <a href="http://www.commonmark.org/help">www.commonmark.org/help</a> for more information.</p>

## Code EX_3

    <p>Visit <a href="http://www.commonmark.org">www.commonmark.org</a>.</p>
    <p>Visit <a href="http://www.commonmark.org/a.b">www.commonmark.org/a.b</a>.</p>
    
이 코드의 실행 결과입니다.
<p>Visit <a href="http://www.commonmark.org">www.commonmark.org</a>.</p>
<p>Visit <a href="http://www.commonmark.org/a.b">www.commonmark.org/a.b</a>.</p>

Trailing punctuation (specifically, ?, !, ., ,, :, *, _, and ~)는 autolink의 일부로 간주되지 않는다.

## Code EX_4

    <p><a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a></p>
    <p><a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a>))</p>
    <p>(<a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a>)</p>
    <p>(<a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a></p>
    
이 코드의 실행 결과입니다.
<p><a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a></p>
<p><a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a>))</p>
<p>(<a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a>)</p>
<p>(<a href="http://www.google.com/search?q=Markup+(business)">www.google.com/search?q=Markup+(business)</a></p>

여는 괄호보다 닫히는 괄호가 더 많을 경우 자동 링크에 포함되지 않는 괄호를 빼버린다.

## Code EX_5

    <p><a href="http://www.google.com/search?q=(business))+ok">www.google.com/search?q=(business))+ok</a></p>
    
이 코드의 실행 결과입니다.
<p><a href="http://www.google.com/search?q=(business))+ok">www.google.com/search?q=(business))+ok</a></p>

Code EX_4는 autolink의 마지막이 )로 끝날 때에만 적용됩니다.

## Code EX_6

    <p><a href="http://www.google.com/search?q=commonmark&amp;hl=en">www.google.com/search?q=commonmark&amp;hl=en</a></p>
    <p><a href="http://www.google.com/search?q=commonmark">www.google.com/search?q=commonmark</a>&amp;hl;</p>
    
이 코드의 실행 결과입니다.
<p><a href="http://www.google.com/search?q=commonmark&amp;hl=en">www.google.com/search?q=commonmark&amp;hl=en</a></p>
<p><a href="http://www.google.com/search?q=commonmark">www.google.com/search?q=commonmark</a>&amp;hl;</p>

자동 링크가 세미콜론(;)으로 끝나는 경우 엔티티 참조와 유사한지, 이전 텍스트가 하나 이상의 영숫자 뒤에 있는지 확인합니다.  
만약 그렇다면 자동 링크에서 제외됩니다.

## Code EX_7

    <p><a href="http://www.commonmark.org/he">www.commonmark.org/he</a>&lt;lp</p>
    
 이 코드의 실행 결과입니다.
 <p><a href="http://www.commonmark.org/he">www.commonmark.org/he</a>&lt;lp</p>  
 
 <이 나오면 즉시 autolink에서 제외됩니다.
 
## Code EX_8

    <p><a href="http://commonmark.org">http://commonmark.org</a></p>
    <p>(Visit <a href="https://encrypted.google.com/search?q=Markup+(business)">https://encrypted.google.com/search?q=Markup+(business)</a>)</p>
    
이 코드의 실행 결과입니다.
<p><a href="http://commonmark.org">http://commonmark.org</a></p>
<p>(Visit <a href="https://encrypted.google.com/search?q=Markup+(business)">https://encrypted.google.com/search?q=Markup+(business)</a>)</p>

## Code EX_9

    <p><a href="mailto:foo@bar.baz">foo@bar.baz</a></p>
    
이 코드의 실행 결과입니다.
<p><a href="mailto:foo@bar.baz">foo@bar.baz</a></p>

Extended email autolink Rules  
영숫자 또는 ., -, _ 또는 +인 하나 이상의 문자입니다.  
@ 기호입니다.  
영숫자 또는 - 또는 _, 마침표(.)로 구분된 하나 이상의 문자입니다.  
적어도 하나의 마침표가 있어야 합니다.  
마지막 문자는 - 또는 _ 중 하나일 수 없습니다.

## Code EX_10

    <p>hello@mail+xyz.example isn't valid, but <a href="mailto:hello+xyz@mail.example">hello+xyz@mail.example</a> is.</p>
    
이 코드의 실행 결과입니다.
<p>hello@mail+xyz.example isn't valid, but <a href="mailto:hello+xyz@mail.example">hello+xyz@mail.example</a> is.</p>

+는 @의 뒤에 올 수 없고, 앞에만 올 수 있습니다.

## Code EX_11

    <p><a href="mailto:a.b-c_d@a.b">a.b-c_d@a.b</a></p>
    <p><a href="mailto:a.b-c_d@a.b">a.b-c_d@a.b</a>.</p>
    <p>a.b-c_d@a.b-</p>
    <p>a.b-c_d@a.b_</p>
    
이 코드의 실행 결과입니다.
<p><a href="mailto:a.b-c_d@a.b">a.b-c_d@a.b</a></p>
<p><a href="mailto:a.b-c_d@a.b">a.b-c_d@a.b</a>.</p>
<p>a.b-c_d@a.b-</p>
<p>a.b-c_d@a.b_</p>

. , _ , -은 @ 앞뒤에 모두 올 수 있지만, .만이 이메일 주소의 맨 뒤에 올 수 있습니다.

# Disallowed Raw HTML

\<title>
\<textarea>
\<style>
\<xmp>
\<iframe>
\<noembed>
\<noframes>
\<script>
\<plaintext>

이 HTML 태그들은 렌더링 시 필터링을 거칩니다.  
즉, <이 \&lt;로 필터링됩니다.

## Code EX_1

    <p><strong> &lt;title> &lt;style> <em></p>
    <blockquote>
      &lt;xmp> is disallowed.  &lt;XMP> is also disallowed.
    </blockquote>
   
이 코드의 실행 결과입니다.
<p><strong> &lt;title> &lt;style> <em></p>
<blockquote>
  &lt;xmp> is disallowed.  &lt;XMP> is also disallowed.
</blockquote>
