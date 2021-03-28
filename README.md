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
  
