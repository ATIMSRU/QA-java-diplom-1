# Stellar Burgers Unit Tests

## Описание проекта
Этот проект содержит **юнит-тесты** для Java-приложения **Stellar Burgers**, отвечающего за сборку заказов с бургерами.  
Тесты покрывают основные классы модели данных: `Bun`, `Ingredient`, `Burger`, `IngredientType`, а также их взаимодействие.

## **Тестируемые сценарии**
Проект покрывает тестирование следующих классов:

### **1. Тестирование класса `Bun`**
- ✅ Корректное создание булочки с именем и ценой
- ✅ Корректность геттеров (`getName()`, `getPrice()`)

### **2. Тестирование класса `Ingredient`**
- ✅ Корректное создание ингредиента с типом (`SAUCE` или `FILLING`), названием и ценой
- ✅ Корректность геттеров (`getName()`, `getPrice()`, `getType()`)

### **3. Тестирование класса `IngredientType`**
- ✅ Проверка наличия двух типов ингредиентов (`SAUCE`, `FILLING`)

### **4. Тестирование класса `Burger`**
- ✅ Добавление булочки в бургер (`setBuns()`)
- ✅ Добавление ингредиента (`addIngredient()`)
- ✅ Удаление ингредиента (`removeIngredient()`)
- ✅ Перемещение ингредиента (`moveIngredient()`)
- ✅ Расчёт стоимости бургера (`getPrice()`)
- ✅ Генерация чека (`getReceipt()`, проверка соответствия формата вывода)

## **Технологии в проекте**
| Технология   | Версия  |
|-------------|---------|
| **Java**    | 11      |
| **JUnit**   | 4.13.2  |
| **Mockito** | 4.5.1   |
| **Maven**   | 3.9.0   |
| **Jacoco**  | 0.8.7   |
| **AssertJ** | 3.24.2  |

## **Установка и запуск проекта**

### **1. Подготовка**
Перед началом работы убедитесь, что у вас установлены:
- **Java 11**
- **Maven 3.9.0**
- **IDE с поддержкой Maven** (например, IntelliJ IDEA)

### **2. Клонирование репозитория**
```
git clone git@github.com:USERNAME/QA-java-diplom-1.git
cd QA-java-diplom-1
```
### **3. Убедитесь, что все зависимости проекта установлены.**
Для этого выполните команду:

```
mvn clean install
```
### **4. Для запуска тестов используйте следующую команду:**

```
mvn clean test
```

### **5. Для генерации Allure-отчёта выполните команду:**
```
mvn jacoco:report
```