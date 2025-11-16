# المختار الصرفي / Morphological Selector

<div dir="rtl">

أداة متقدمة لتحليل الصرف العربي (Morphological Analysis) مع قاعدة بيانات شاملة للأوزان والوسوم والسوابق واللواحق.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

</div>

## المميزات

- **تحليل صرفي شامل**: تحليل الأسماء والأفعال
- **قاعدة بيانات شاملة**: أوزان الأسماء والأفعال، السوابق واللواحق
- **نظام الوسم**: تصنيف الكلمات حسب نوعها
- **قلب الأوزان**: تحويل الأوزان بين الصيغ المختلفة
- **واجهة رسومية**: واجهة مستخدم سهلة الاستخدام
- **تقارير مفصلة**: تقارير تحليلية شاملة
- **نظام تخزين مؤقت**: تسريع التحليل المتكرر

## المتطلبات

- Python 3.7 أو أحدث
- PyQt6 (للواجهة الرسومية - إن وجدت)

## التثبيت

1. استنسخ المستودع:
```bash
git clone https://github.com/ayzem88/morphological-selector.git
cd morphological-selector
```

2. ثبت المتطلبات:
```bash
pip install -r requirements.txt
```

3. **ملاحظة مهمة**: البرنامج يحتاج ملف `morphology.db` (قاعدة البيانات الصرفية) للعمل. هذا الملف كبير جداً (>100MB) ولم يتم رفعه على GitHub.

   **الحلول**:
   - يمكنك إنشاء قاعدة البيانات من ملفات `قواعد البيانات/*.txt` الموجودة في المستودع
   - أو طلب الملف من المطور
   - البرنامج سيعمل بدون قاعدة البيانات لكن مع وظائف محدودة

## الاستخدام

### التشغيل

```bash
python run.py
```

أو مباشرة:
```bash
python "0.5 المختار الصرفي.py"
```

## الملفات

- `0.5 المختار الصرفي.py`: الملف الرئيسي
- `run.py`: ملف التشغيل المبسط
- `morphology.db`: قاعدة البيانات الصرفية
- `قواعد البيانات/`: مجلد قواعد البيانات النصية
  - `أوزان_الأسماء.txt`
  - `أوزان_الأفعال.txt`
  - `الوسم.txt`
  - `سوابق ولواحق_أسماء.txt`
  - `سوابق ولواحق_أفعال.txt`
  - `قلب الأوزان.txt`
  - `الخريطة.txt`
- `cache/`: مجلد التخزين المؤقت
- `reports/`: مجلد التقارير

## الميزات التفصيلية

### تحليل الأسماء
- تحديد وزن الاسم
- كشف السوابق واللواحق
- تصنيف حسب الوسم

### تحليل الأفعال
- تحديد وزن الفعل
- كشف السوابق واللواحق
- تصنيف حسب الوسم

### قلب الأوزان
- تحويل الأوزان بين الصيغ المختلفة
- دعم التحويلات المعقدة

## الاختبار

```bash
# تثبيت متطلبات التطوير
pip install -r requirements-dev.txt

# تشغيل الاختبارات
python -m pytest tests/
```

## المساهمة

نرحب بمساهماتكم! راجع [دليل المساهمة](CONTRIBUTING.md) للتفاصيل.

## الترخيص

هذا المشروع مرخص تحت [MIT License](LICENSE) - راجع ملف LICENSE للتفاصيل.

## المطور

تم تطوير هذا المشروع بواسطة **أيمن الطيّب بن نجي** ([ayzem88](https://github.com/ayzem88))

## التواصل

للاستفسارات أو المساهمة، يمكنك التواصل معي عبر:
- البريد الإلكتروني: [aymen.nji@gmail.com](mailto:aymen.nji@gmail.com)

## التطوير المستقبلي

- [ ] واجهة رسومية محسّنة
- [ ] دعم المزيد من الأوزان
- [ ] تحسين دقة التحليل
- [ ] واجهة سطر الأوامر (CLI)
- [ ] API للاستخدام البرمجي

## الصور

![صورة 1](img-01.png)
![صورة 2](img-02.png)
![صورة 3](img-03.png)

---

# [English]

<div dir="ltr">

## Morphological Selector

An advanced tool for Arabic morphological analysis with a comprehensive database of patterns, tags, prefixes, and suffixes.

![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Features

- **Comprehensive Morphological Analysis**: Analysis of nouns and verbs
- **Comprehensive Database**: Patterns for nouns and verbs, prefixes and suffixes
- **Tagging System**: Classification of words by type
- **Pattern Conversion**: Convert patterns between different forms
- **Graphical Interface**: Easy-to-use user interface
- **Detailed Reports**: Comprehensive analytical reports
- **Caching System**: Speed up repeated analysis

## Requirements

- Python 3.7 or later
- PyQt6 (for graphical interface - if available)

## Installation

1. Clone the repository:
```bash
git clone https://github.com/ayzem88/morphological-selector.git
cd morphological-selector
```

2. Install requirements:
```bash
pip install -r requirements.txt
```

3. **Important Note**: The program needs the `morphology.db` file (morphological database) to work. This file is very large (>100MB) and was not uploaded to GitHub.

   **Solutions**:
   - You can create the database from the `قواعد البيانات/*.txt` files in the repository
   - Or request the file from the developer
   - The program will work without the database but with limited functionality

## Usage

### Running

```bash
python run.py
```

Or directly:
```bash
python "0.5 المختار الصرفي.py"
```

## Files

- `0.5 المختار الصرفي.py`: Main file
- `run.py`: Simplified run file
- `morphology.db`: Morphological database
- `قواعد البيانات/`: Text database folder
  - `أوزان_الأسماء.txt`
  - `أوزان_الأفعال.txt`
  - `الوسم.txt`
  - `سوابق ولواحق_أسماء.txt`
  - `سوابق ولواحق_أفعال.txt`
  - `قلب الأوزان.txt`
  - `الخريطة.txt`
- `cache/`: Cache folder
- `reports/`: Reports folder

## Detailed Features

### Noun Analysis
- Identify noun pattern
- Detect prefixes and suffixes
- Classify by tag

### Verb Analysis
- Identify verb pattern
- Detect prefixes and suffixes
- Classify by tag

### Pattern Conversion
- Convert patterns between different forms
- Support for complex conversions

## Testing

```bash
# Install development requirements
pip install -r requirements-dev.txt

# Run tests
python -m pytest tests/
```

## Contributing

We welcome contributions! See [Contributing Guide](CONTRIBUTING.md) for details.

## License

This project is licensed under [MIT License](LICENSE) - see the LICENSE file for details.

## Developer

Developed by **Ayman Al-Tayyib Ben Naji** ([ayzem88](https://github.com/ayzem88))

## Contact

For inquiries or contributions, you can contact me via:
- Email: [aymen.nji@gmail.com](mailto:aymen.nji@gmail.com)

## Future Development

- [ ] Enhanced graphical interface
- [ ] Support for more patterns
- [ ] Improved analysis accuracy
- [ ] Command-line interface (CLI)
- [ ] API for programmatic use

## Screenshots

![Screenshot 1](img-01.png)
![Screenshot 2](img-02.png)
![Screenshot 3](img-03.png)

</div>

