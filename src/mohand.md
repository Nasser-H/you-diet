for /f "tokens=1* delims=/" %a in ('git branch -r ^| findstr /v /c:"->"') do @if not "%b"=="" git branch --track %b origin/%b
