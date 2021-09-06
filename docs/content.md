## 강의 내용을 더 세부적으로 알아가고 싶어서 작성한 Markdown 파일

**content**

- [1. HTML](https://github.com/mnxmnz/Twitter-Clone-Frontend/blob/main/docs/content.md#html)
- [2. CSS](https://github.com/mnxmnz/Twitter-Clone-Frontend/blob/main/docs/content.md#css)
- [3. React](https://github.com/mnxmnz/Twitter-Clone-Frontend/blob/main/docs/content.md#react)
- [4. Next](https://github.com/mnxmnz/Twitter-Clone-Frontend/blob/main/docs/content.md#next)
- [5. Dev](https://github.com/mnxmnz/Twitter-Clone-Frontend/blob/main/docs/content.md#dev)

<br />

### HTML

<br />

#### a (noreferrer noopener)

```tsx
<a href="https://github.com/mnxmnz" target="_blank" rel="noreferrer noopener">
  Made by MinJi
</a>
```

📄 [MDN - HTML](https://developer.mozilla.org/ko/docs/Web/HTML/Element/a)

📄 [Blog - [SEO] target="\_blank" 좀 더 알고 사용하자(noopener, norefferrer, nofollow 차이점에 대해서)](https://webruden.tistory.com/262)

<br />
<hr />
<br />

### CSS

<br />

#### vertical-align

![vertical-align](https://bitsofco.de/content/images/2015/12/Group-1.png)

```tsx
<Input.Search enterButton style={{ verticalAlign: 'middle' }} />
```

📄 [MDN - CSS](https://developer.mozilla.org/ko/docs/Web/CSS/vertical-align)

📄 [W3Schools - CSS](https://www.w3schools.com/cssref/pr_pos_vertical-align.asp)

<br />
<hr />
<br />

### React

#### children (TypeScript)

- TypeScript 환경에서 React children을 사용할 때 children은 `ReactNode` 타입

```tsx
type LayoutProps = {
  children: React.ReactNode;
};

function AppLayout({ children }: LayoutProps) { ... }
```

📄 [TypeScript docs - JSX](https://www.typescriptlang.org/ko/docs/handbook/jsx.html)

📄 [React docs - Children in JSX](https://ko.reactjs.org/docs/jsx-in-depth.html#children-in-jsx)

📄 [React docs - Children API](https://ko.reactjs.org/docs/react-api.html#reactchildren)

<br />

#### useCallback

- 컴포넌트에 props로 넘겨주는 함수는 `useCallback` 사용하기

```tsx
const onChangeId = useCallback(e => {
  setId(e.target.value);
}, []);

<Input name="user-id" value={id} onChange={onChangeId} required />;
```

📄 [React docs - Hooks API](https://ko.reactjs.org/docs/hooks-reference.html#usecallback)

📄 [Blog - React.memo, useCallback 사용으로 렌더링 최적화 하기(feat.React-Native,Redux)](https://velog.io/@shin6403/React.memo-useCallback-사용으로-렌더링-최적화-하기feat.React-NativeRedux)

<br />
<hr />
<br />

### Next

<br />

#### Link tag

```tsx
<Link href="/">
  <a>Home</a>
</Link>
```

📄 [Next docs - next/link](https://nextjs.org/docs/api-reference/next/link)

📄 [Blog - [번역] next/link 공식 문서](https://crong-dev.tistory.com/50)

📄 [Blog - Next.js Link 태그안에 a tag를 안넣어도 왜 잘 작동될까?](https://uchanlee.dev/nextjs/Why-using-a-tag-in-nextjs-Link/)

📄 [Stack Overflow - Next.JS "Link" vs "router.push()" vs "a" tag](https://stackoverflow.com/questions/65086108/next-js-link-vs-router-push-vs-a-tag)

<br />
<hr />
<br />

### Dev

<br />

#### Gutter

![Gutter](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRQjklenrQEIc2uz5DfXlLXE5hQ4n2_EBddIA&usqp=CAU)

![Gutter](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSqY4ZHkGhmXhY0ONelqJJKoxVEqjzqflxJdw&usqp=CAU)

- Gutter 용어 의미 알고 있기

```tsx
<Row gutter={8}> ... </Row>
```

📄 [MDN - Glossary](https://developer.mozilla.org/en-US/docs/Glossary/Gutters)
