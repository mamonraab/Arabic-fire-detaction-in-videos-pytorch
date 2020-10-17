<!-- <div dir="rtl"><a href="https://github.com/ellerbrock/open-source-badges/"><img src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103" alt="Open Source Love"></a><a href="https://firstcontributions.herokuapp.com">[<img align="left" width="150" src="../assets/join-slack-team.png">](https://join.slack.com/t/firstcontributors/shared_invite/enQtNjkxNzQwNzA2MTMwLTVhMWJjNjg2ODRlNWZhNjIzYjgwNDIyZWYwZjhjYTQ4OTBjMWM0MmFhZDUxNzBiYzczMGNiYzcxNjkzZDZlMDM)</a></div> -->

[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
[<img align="right" width="150" src="../assets/join-slack-team.png">](https://join.slack.com/t/firstcontributors/shared_invite/enQtMzE1MTYwNzI3ODQ0LTZiMDA2OGI2NTYyNjM1MTFiNTc4YTRhZTg4OWZjMzA0ZWZmY2UxYzVkMzI1ZmVmOWI4ODdkZWQwNTM2NDVmNjY)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Open Source Helpers](https://www.codetriage.com/roshanjossey/first-contributions/badges/users.svg)](https://www.codetriage.com/roshanjossey/first-contributions)


# <div dir="rtl">المقدمة </div>

<div dir="rtl">
يعتبر الفيدو من المصادر المهمة للمعلومات ولبناء انظمة مختلفة    ونحن هنا سنستخدم الفيديو للكشف عن حالات العنف سواء كان فيديو من كامرات مراقبة او فيديو  في مقطع فلم او عبر الانترنت<br>

كبداية  هنالك ثلاثة طرق  شائعه للتعامل مع كشف  الحركة او معالجة الفيديو بالتعلم العميق
وهذه الطرق
<br>
(Conv3d) 
<br>
(Convlstm) 

<br>
(Conv  +  lstm) :   هذه الطريقة تتيح لنا استخدام  شبكة كونفليوشن مدربة مسبقا  لتحسين النتائج وهي الطريقة الاكثر شيوعا عندما يكون  لدينا عدد بيانات قليل وايضا قدرة الحاسوب من ناحية كارت الشاشة قليلة  ولذلك سنقوم بعمل الشرح على هذه الطريقة وايضا لن هذه الطريقة تحتج جهد خاص لتطويعها وفق بيئة  pytorch



<br>  ماذا ستتعلم من هذا المقال

<br> 1-  بناء كلاس  خاص لقراءة المحتوى الفيديوي  للpytorch

<br> 2-  بناء  كلاس خاص  لتوزيع الصور من الفيديو الواحد على الكونفليوشن الاعتيادية    مشابة  لل  time-distrbution in keras

<br> 3-  استخدمات  الlstm   بسهولة بداخل   ال  sequnatil mode in pytorch
</div>

# <div dir="rtl"> المتطلبات الاساسية </div>

<div dir="rtl">


<br> 1-  ان تكون بمستوى متوسط  بالباي تورش   اي ان تستطيع على الاقل انشاء مودل وتدريبة  

<br> 2-  تكون المكتبات التالية مثبته لديك   pytorch , opencv , pandas

<br> 3-  البيانات المستخدمة بالتدريب يمكنك تحميلها وايجادها من الروابط التالية علما انني قمت بدمجها ثلاثتها وتدريب المودل عليها
 (Movies Fight Detection Dataset https://academictorrents.com/details/70e0794e2292fc051a13f05ea6f5b6c16f3d3635 ) , (Hockey Fight Detection Dataset https://academictorrents.com/details/38d9ed996a5a75a039b84cf8a137be794e7cee89 ) , and (VIOLENT-FLOWS DATABASE https://www.openu.ac.il/home/hassner/data/violentflows/ )

</div>

<div dir="rtl">
قراءة ومشاهدة التعليمات المتوفرة على الإنترنت ستساعدك حتماً، لكنك ستستفيد أكثر إذا استطعت المساهمة في مشروع دون الخوف من الوقوع في الخطأ. هذا المشروع يركز على توفير التوجيهات والتعليمات البدائية لإتمام أول مساهمة لك.
تذكر أن الخطأ متوقع والهدف أن تتجاوز الخطأ في هذه البيئة، نريد منك أن تكون مسترخيا ومتابعا الخطوات المتوفرة لإتمام مشاركتك الأولى. نعدك ستستمع بذلك.
</div>


<div dir="rtl">
إذا لم يكن لديك git على الجهاز الخاص بك،<a href="https://help.github.com/articles/set-up-git/">قم بتثبيته من هنا</a>
</div>

## <div dir="rtl"> افرق هذا المشروع - Fork this Repository </div>
<img style="float: left;" width="300" src="../assets/fork.png" alt="fork this repository" />
<div dir="rtl">
افرق هذا المشروع بالضغط على زر Fork في أعلى هذه الصفحة.
من خلال ذلك ستنشأ نسخة من هذا المشروع على حسابك الخاص.
</div>

## <div dir="rtl"> استنسخ هذا المشروع - Clone the repository </div>

<img style="float: left;" width="300" src="../assets/clone.png" alt="clone this repository" />

<div dir="rtl">
استنسخ هذا المشروع على جهازك.
انقر على زر Clone ثم انقر على أيقونة Copy to clipboard
</div>
<img style="float: left;" width="300" src="../assets/copy-to-clipboard.png" alt="copy URL to clipboard" />
<div dir="rtl">
افتح الطرفية واكتب الأمر التالي:
</div>

```
git clone "url you just copied"
```

<div dir="rtl">قم باستبدال "url you just copied" بالرابط الذي نسخته من الخطوة السابقة، هذا الرابط يحتوي على المشروع.</div>

<div dir="rtl">على سبيل المثال:</div>

```
git clone https://github.com/this-is-you/first-contributions.git
```

<div dir="rtl">
في هذا المثال لاحظ 'this-is-you' سيكون اسم حسابك في موقع github يليه رابط المشروع الذي فرقته في أول خطوة، هذا الأمر سينسخ محتويات المشروع على جهازك لتتمكن من التعديل عليه بحرية.
</div>
<br>

## <div dir="rtl">  إنشاء فرع - Create a branch </div>


<div dir="rtl"> انتقل إلى المجلد الذي يحتوي على المشروع عن طريق الأمر التالي: </div>

```
cd first-contributions
```

<div dir="rtl"> الآن قم بإنشاء فرع عن طريق الأمر التالي: </div>

```
git checkout -b "add-your-name"
```

<div dir="rtl">اسمك بدل add-your-name</div>

<div dir="rtl">على سبيل المثال:</div>

```
git checkout -b "add-alonzo-church"
```

<br>

## <div dir="rtl">قم بإجراء التعديلات المطلوبة وأتممها</div></h2>

<div dir="rtl">
الآن قم بفتح الملف "Contributors.md" في محرر النصوص المفضل لديك وأضف اسمك ثم احفظ الملف.
بعد ذلك اذهب إلى الطرفية واكتب الأمر هذا<code>git status</code> هذا الأمر سيظهر لك التغيرات التي حدثت في المشروع.
لإضافة هذه التغييرات قم بإضافتها عن طريق هذا الأمر <code>git add</code>.
</div>

```
git add Contributors.md
```

<div dir="rtl">الآن قم بإتمام التغييرات باستخدام الأمر <code>git commit</code>.</div>

```
git commit -m "Add <your-name> to Contributors list"
```

<div dir="rtl"> استبدل <code>&#60;your-name&#62;</code> باسمك. </div>
<br>

## <div dir="rtl"> ارفع التغييرات إلى github - Push changes to Github </div>

<div dir="rtl">ارفع التغيررات عن طريق الأمر <code>git push</code></div>

```
git push origin "add-your-name"
```

<div dir="rtl">استبدل <code>&#60;add-your-name&#62;</code> باسم الفرع الذي أنشأته من قبل.</div>


<br>
<h2 id="سلم-تغيراتك-للمراجعة"><a name="سلم-تغيراتك-للمراجعة" href="#سلم-تغيراتك-للمراجعة"></a><div dir="rtl">سلم تغيراتك للمراجعة</div></h2>


<div dir="rtl">في صفحة المشروع الخاصة بك يوجد زر <code>Compare &amp; pull request</code>. اضغط على هذا الزر.</div>

<img style="float: left;" src="../assets/compare-and-pull.png" alt="create a pull request" />

<div dir="rtl">والآن سلم طلبك لتتم مراجعته </div>

<img style="float: left;" src="../assets/submit-pull-request.png" alt="submit pull request" />

<div dir="rtl">بعد المراجعة سوف أقوم بدمج تغيرراتك إلى الفرع الرئيس في المشروع. سيتم تنبيهك عن طريق البريد الإلكتروني بذلك.</div>

<div dir="rtl">الفرع الرئيس الخاص بك لن يحتوي على هذه التغيررات. عليك مزامنته مع الفرع الرئيس عن طريق الخطوات التالية.</div>

## <div dir="rtl">مزامنة نسختك مع المشروع الرئيسي</div>

 <div dir="rtl">الخطوة الأولى، انتقل إلى الفرع الرئيس.</div>

```
git checkout master
```

 <div dir="rtl">ثانياً، أضف رابط مشروعي كـ<code>upstream remote url</code>.</div>
 
```
git remote add upstream https://github.com/Roshanjossey/first-contributions
```

<div dir="rtl">بهذه الطريقة نخبر git أن هناك نسخة أخرى من هذا المشروع في هذا الرابط ونسميها <code>upstream</code>.
بعد أن أوافق على تغيرراتك، قم بسحب النسخة الجديدة من المشروع عن طريق الأمر التالي:
</div>

```
git fetch upstream
```

<div dir="rtl">هنا سنقوم بسحب جميع التغييرات من <code>(upstream remote)</code>. والآن، عليك أن تدمج التحديثات الجديدة من فرعي إلى فرعك الرئيس.</div>

```
git rebase upstream/master
```

<div dir="rtl">وهنا تطبق التغييرات إلى الفرع الرئيس. إذا رفعت التغييرات لفرعك الرئيس سيتم تحديث مشروعك</div>

```
git push origin master
```

<div dir="rtl">لاحظ أنك ترفع إلى <code>remote</code> اسمه <code>origin</code>.</div>
<br>

## <div dir="rtl">توجيهات بإستخدام أدوات أخرى</div>

|<a href="../github-desktop-tutorial.md"><img alt="GitHub Desktop" src="https://desktop.github.com/images/desktop-icon.svg" width="100"></a>|<a href="../github-windows-vs2017-tutorial.md"><img alt="Visual Studio 2017" src="https://upload.wikimedia.org/wikipedia/commons/c/cd/Visual_Studio_2017_Logo.svg" width="100"></a>|<a href="../gitkraken-tutorial.md"><img alt="GitKraken" src="../assets/gk-icon.png" width="100"></a>|
|---|---|---|
|[GitHub Desktop](../github-desktop-tutorial.md)|[Visual Studio 2017](../github-windows-vs2017-tutorial.md)|[GitKraken](../gitkraken-tutorial.md)|


