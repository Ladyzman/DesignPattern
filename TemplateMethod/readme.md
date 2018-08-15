## Template Method


樣板方法模式 學習筆記

### 定義：
    在父類別定義演算法的流程架構，在子類別為流程步驟提供方法實現。
    讓子類別在不改變演算法架構及順序的情況下，重新定義演算法中的某些步驟。

### 目的：
    1. 提高code的擴充性，使用靈活性
    2. 減少重複code和大量的覆寫
    3. 不希望改變演算法的架構

### 架構：
    抽象的父類別：演算法流程，抽象方法。
    具體的子類別：依步驟細節，實作方法。

### 特徵：
    1. 抽象方法(Abstract Method)
        ● 父類別宣告，子類別實現
    2. 具體方法(Concrete Method)
        ● 父類別宣告並實現，子類別繼承或覆寫
    3. 掛鉤方法(Hook Method)
        ● 父類別宣告並實現，通常是空實現。
        ● 子類別進行擴充，用來達到對父類別的反向控制。
        ● 通常回傳值為 boolean type。

### 優缺點：
    ● 優點：
        1. 符合開放封閉原則和單一和單一職責原則
        2. 實現反向控制，藉由掛鉤方法來處理特殊情況且不破壞演算法本身的流程。
    ● 缺點：
        1.每一個抽象方法都需實作，當有多個子類別就會有多個實作，導致系統太過龐大。



參考：
1. <a href = "https://blog.csdn.net/lovelion/article/details/8299794"> 模板方法模式深度解析 </a>
2. <a href = "https://sophia.javeriana.edu.co/~cbustaca/docencia/DSBP-2018-01/recursos/Erich%20Gamma,%20Richard%20Helm,%20Ralph%20Johnson,%20John%20M.%20Vlissides-Design%20Patterns_%20Elements%20of%20Reusable%20Object-Oriented%20Software%20%20-Addison-Wesley%20Professional%20(1994).pdf"> Design Patterns Elements Of Reusable Object-oriented Software @345 </a>




