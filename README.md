# 글쓰기 에디터 - TOAST UI 샘플 코드
---------------------------------------
## 공식문서
- https://nhn.github.io/tui.editor/latest/
---------------------------------------
## 적용방법
### CDN 사용
---------------------------------------
#### BOOTSTRAP
```
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
```

```
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
```

#### TOAST UI
```
<link rel="stylesheet" href="https://uicdn.toast.com/editor/latest/toastui-editor.min.css" />
```

---------------------------------------

### html body 영역

```
<body>
    <div id="editor"></div>
    <script src="https://uicdn.toast.com/editor/latest/toastui-editor-all.min.js"></script>
    <script>
        const Editor = toastui.Editor;
        const editor = new Editor({
            el: document.querySelector('#editor'),
            height: '500px',
            initialEditType: 'wysiwyg',
            previewStyle: 'vertical'
        });
        editor.getMarkdown();
    </script>
</body>
```

## 기본 옵션
- height: 문자열의 높이 ex 300px / auto
- initialEditType: 초기 유형 markdown,wysiwyg   
(markdown은 md언어가 같이 표기됨)