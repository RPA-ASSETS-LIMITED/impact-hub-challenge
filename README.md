# 🧪 Тестове завдання: ImpactHub

Це завдання створене для оцінки твоїх навичок у **рефакторингу існуючого проєкту**, оптимізації компонентів і структурі коду. Можеш також реалізувати фічу (не обов’язково).

---

## 📌 Загальна інформація

Проєкт реалізовано на базі:

- `React 18` + `Vite`
- `Redux Toolkit`
- `TailwindCSS`
- `React Router v6`
- `React Hook Form`, `Framer Motion`, `Recharts`
- `Jest + React Testing Library`

Код структуровано в `pages`, `components`, `components/ui`, `hooks`, `constants`.

---

## ✅ Частина 1 (ОБОВ’ЯЗКОВО): **Рефакторинг існуючого коду**

### 🎯 Мета

Скоротити обсяг коду та зробити його легшим для підтримки. Виявити дублювання, покращити архітектуру, спростити компоненти і підготувати структуру до масштабування.

---

### 🔧 Очікування

- **Скорочення обсягу коду на 25–40%**
- Винесення повторюваної логіки в:
  - **кастомні хуки** (`useVerificationSteps`, `useCarousel`, `useMissionFilter`)
  - **уніфіковані компоненти** (`Section`, `Block`, `StepCard`)
- Уніфікація стилів Tailwind через пропси або класи
- Оптимізація обробки форм (`React Hook Form`) через хук або shared-компонент
- Упорядкування структури файлів і компонентів

---

### 📂 Що саме рефакторити

1. **Компоненти `pages/homepage/components/`**
   - `HowItWorks`, `ImpactCalculator`, `PartnerSpotlight`, `TestimonialsCarousel` — дублювання структур секцій

2. **Процес верифікації `pages/organization-verification/components/`**
   - Схожі компоненти по шаблону — можна зробити загальну "step"-структуру

3. **UI-компоненти**
   - `Button`, `Header`, `Input` — оптимізувати стилі, уніфікувати пропси

---

### 📄 Що очікується

- Коміти `refactor: ...`
- Файл `REFACTOR_NOTES.md` з поясненням:
  - Що переписано, чому, наскільки скорочено
- Повна працездатність і візуальна відповідність сайту

---

## ➕ Частина 2 (ОПЦІЙНО): **Нова функція — Dashboard прогресу верифікації**

#### User Story

> Як організація, я хочу бачити свій прогрес верифікації, щоб розуміти, які кроки я завершив, а які залишилися.

---

### 📌 Acceptance Criteria

1. Нова сторінка/секція `VerificationProgress`
   - Компонент з прогрес-барами або кроками (`Step 1 of 3`)
   - Візуалізація: кругові/лінійні індикатори (Recharts або простий SVG)

2. Мок-дані або локальний Redux-стан

3. UX: кнопки `Continue`, `Edit`, `Go to step`, `Submit verification`

---

## ⏱ Орієнтовний час

- Рефакторинг: **1–2 години**
- Фіча (опціонально): **1–2 години**

---

## 🔁 Як здати

- Репозиторій або архів з комітами:
  - `refactor: ...`
  - `feat: ...` (якщо є фіча)
- `REFACTOR_NOTES.md`
- Якщо додано dashboard — `DASHBOARD_README.md`

---

## 🧠 Поради

- Не бійся DRY-ити: якщо 2+ компоненти схожі — узагальни
- Якщо повторюється UI/JSX/форма — винеси в `shared/` або `hooks/`
- Tailwind-класи — краще через пропси, ніж дублювати
- Головне — зменшити складність і покращити масштабованість

---

Успіхів! 🚀
