---
lang: he-IL
layout: wiki
section: twilightmenu
category: customization
title: גופנים מותאמים אישית
description: כיצד להשתמש בפונטים מותאמים אישית עבור TWiLight Menu++
---

TWiLight Menu++ יכול להשתמש בגופנים מותאמים אישית בפורמט NFTR (Nitro FonT Resource). הם ישומו בהגדרות, בכותרות של המדריכים ובערכות הנושא של הNintendo DSi, Nintendo 3DS, SEGA Saturn ושל הHomebrew Launcher.

### מידע על הגופנים הכלולים
יש שלושה גופנים כלולים בTWiLight Menu++. בזמן שTWiLight Menu++ רץ במצב DSi, הם כוללים את כל התויים הנדרשים לשפות שTWiLight תורגם אליהם, אבל כאשר הם רצים במצב DS הם יותר מוגבלים בגלל מגבלות RAM. הם כלהלן:
- ברירת מחדל: גופן זה משתמש בגופן הרשמי של הDSi מאחר וזה הוא הגופן העיקרי ותומך בכל התווים בשימוש בTWiLight Menu++ בכל השפות במצב DS
- סינית (מופשטת): גופן זה משתמש בNoto Sans CS בתור הגופן העיקרי, יש לו באופן מובהק יותר תווים של סינית (מופשטת) במצב DS, במחיר של תווים עבור שפות אחרות
- קוראינית: גופן זה זהה לברירת המחדל במצב DSi, אבל במצב DS יש לו סט שלם יותר של הנגול, במחיר של תווים עבור שפות אחרות

### מבנה תיקייה
גופנים מותאמים אישית נטענים מ`sd:/_nds/TWiLightMenu/extras/fonts/[font name]/[font file].nftr`, כשה`[font name]` הוא שם הגופן לבחירתכם ו `[font file].nftr` הוא אחד מהבאים:
- `large-ds.nftr`, `large-dsi.nftr` או `large.nftr`: הגופן הגדול יותר המשמש לכותרות
- `small-ds.nftr`, `small-dsi.nftr` או `small.nftr`: הגופן הקטן יותר המשמש לשאר הטקסט

לקבצי ה`-ds` and `-dsi` יש עדיפות גבוהה יותר מהקבצים הרגילים ואם הם ימצאו, TWiLight Menu++ ישתמש בהם במצב DS או במצב DSi בהתאם.

### יצירת גופנים מותאמים אישית
ניתן ליצור גופנים משלכם באמצעות כלי כגון [nftr-editor](https://pk11.us/nftr-editor/) של Pk11. על מנת ליצור מחדש את אחד מהגופנים של TWiLight Menu++ באמצעותו:
1. טענו את קובץ הNFTR לnftr-editor
1. רשמו את השמותש ל הגופנים שאתם רוצים על פי סדר עדיפויות בתיבת הטקסט `Input font`, מופרדים בפסיק
   - ניתן לראות תצוגה מקדימה של הפונטים בתיבת הטקסט בצד שמאל ואת הNFTR הנוכחי בתיבת הטקסט התחתונה
1. לחצו על `Generate from font`, בחרו ב`OK` על מנת ליצור מחדש תווים קיימים ו`Cancel` על מנת ליצור מחדש את תווי הכפתור המיוחדים (לדוגמת &#xE000;)
1. לחצו על `Save`, וחזרו על הפעולה עבור שאר הגדלים
