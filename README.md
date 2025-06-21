# Face Recognition with CNN & Haar Cascade

Проект по распознаванию лиц в реальном времени с использованием каскадов Хаара для детекции и сверточной нейросети (CNN) для классификации.

---

## Содержимое проекта

| Файл/Изображение            | Назначение                                    |
|-----------------------------|-----------------------------------------------|
| `face_recognition.ipynb`    | Основной код: захват камеры, распознавание лиц|
| `save_data.ipynb`           | Сохранение изображений лиц для обучения       |
| `diagram_1_general_architecture.png` | Общая архитектура системы         |
| `diagram_4_real_time_testing.png`    | Алгоритм работы в реальном времени |
| `diagram_5_classification_logic.png` | Логика классификации CNN           |

---

## Как работает система

1. Загружается обученная модель CNN
2. Открывается камера
3. Захватываются кадры
4. На каждом кадре:
   - Детектируется лицо (алгоритм Haar)
   - Лицо обрезается, масштабируется и нормализуется
   - Подается в модель CNN
   - Выводится имя или метка "Неизвестный"
5. Отображается результат на экране

---

## Диаграммы

### Архитектура системы
![image](https://github.com/user-attachments/assets/c5ada3f7-7635-45cd-bacf-41ea7e7af2e8)

### Поток в реальном времени
![image](https://github.com/user-attachments/assets/c3e61d86-874b-4b0e-998f-fae3a2451ff6)

### Логика классификации
![image](https://github.com/user-attachments/assets/35c6cb76-f907-45b8-810e-8814023df173)

---

## Результат
![image](https://github.com/user-attachments/assets/c24f2f96-f565-4e8e-8f2d-6a1e4d262ac9)
![image](https://github.com/user-attachments/assets/453d1e92-6e47-4a08-9627-e2dfd17a69cf)

---

## Как запустить

1. Установи зависимости:
```bash
pip install opencv-python tensorflow numpy
