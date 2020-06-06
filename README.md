# <div dir="rtl">تعمّق في التعلّم العميق</div>

<div dir="rtl">
هذه النسخة العربية هي ترجمة بتصّرف للنسخة الإنجليزية من كتاب "Dive into deep learning" نرجو أن تنفع القرّاء العرب و تساهم في تحفيز التنمية في الدول العربية.
</div>

### Results of Arabic/RTL support investigation so far:

The d2lbook package used to generate the dive into deep learning book requires:
* Being installed within a conda environment because it uses a mixture of dependencies that cannot be handled properly using pip alone.
* The current theme for the book doesn't support Arabic direction (RTL). setting `language = "ar"` is overwritten why `d2lbook build html`.
    - Potentially clone the d2lbook repo and make the necessary changes to support Arabic. 
        1. Enable setting language = "ar" and see if that results in a correctly rendered Arabic document.
        2. Define what needs to be changed to make the current theme support RTL/Arabic
