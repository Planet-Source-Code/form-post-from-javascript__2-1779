<div align="center">

## Form Post from Javascript


</div>

### Description

Heres and example of using javascript to submit a form post.

http://www.truegeeks.com/asp/mam/osdoc/osframe.asp
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[N/A](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/empty.md)
**Level**          |Beginner
**User Rating**    |3.0 (9 globes from 3 users)
**Compatibility**  |
**Category**       |[Forms Validation Processing](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/forms-validation-processing__2-76.md)
**World**          |[Java](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/java.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/form-post-from-javascript__2-1779/archive/master.zip)





### Source Code

```
<HTML>
<BODY>
<SCRIPT LANGUAGE=javascript>
function dosubmit() {
document.forms[0].action = "test3.asp"
document.forms[0].method = "POST"
document.forms[0].submit()
}
</script>
<FORM NAME=FORM1>
<INPUT TYPE=BUTTON NAME=BT1 VALUE="Some value to post" onClick="dosubmit()"><br>
</FORM>
</BODY>
</HTML>
The "Test3.asp" code:
<HTML>
<BODY>
<H2>Test Post from Javascript</H2>
<%
BT1 = request.form("BT1")
if BT1 = "" then
  response.write "BT1 value not posted."
else
  response.write "BT1 value posted = " & BT1
endif
%>
</BODY>
</HTML>
Top of Form 1
Bottom of Form 1
```

