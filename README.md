# React Modal Component

## 1. Introduction

This library is a react component to display a custom modal inside your app.

## 2. Installation

Run the following command :
`npm install react-modal-jbc`

## 3. Usage

```
import { useState } from "react";
import Modal from "react-modal-jbc"

function App() {
  const [showModal, setShowModal] = useState(false);

  return (
    <main>
      <Modal
        isShow={showModal}
        isClose={() => {
          setShowModal();
        }}
        isFading={true}
        isSlideIn={true}
        isCloseBtn={true}
        isCloseBtnInsideModal={true}
        borderRadius=".5"
      >
        <div className="dialog-body">
          <h1>Title</h1>
        </div>
      </Modal>
    </main>
  );
}

export default App;
```

## 4. Props

- `isShow`: Display a modal or not (Bool)
- `isClose`: Close modal function (Func)
- `isFading`: Add fade effect on true (Bool)
- `isSlideIn`: Add SlideIn effect on true (Bool)
- `isCloseBtn`: Display Close icon on true (Bool)
- `isCloseBtnInsideModal`: Display Close btn inside a footer on true (Bool)
- `borderRadius`: Set Modal border radius in rem unit (String)
- `children`: Display the content (JSX Element)

## 5. Styles
For better visual render make sure to import the Bootstrap CSS file to apply the default styles :

Run the following command :
`npm i bootstrap`

Then import CSS to your main file : `import "bootstrap/dist/css/bootstrap.min.css";`

Then you can customize styles by overriding default CSS classes

## 5. Author

Jean-Baptiste Calzia
