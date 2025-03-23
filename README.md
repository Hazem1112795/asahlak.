<div class="container" id="step2" style="display: none;">
    <h2>تم تسجيل الدخول بنجاح</h2>
    <p>مرحبًا بك في الصفحة الثانية</p>
    <button onclick="goToMainPage()">الصفحة الرئيسية</button>
</div>  

<script>
    function toggleMode() {
        document.body.classList.toggle("dark-mode");
    }

    function nextStep() {
        const firstName = document.getElementById('firstName').value.trim();
        const lastName = document.getElementById('lastName').value.trim();
        const phone = document.getElementById('phone').value.trim();

        if (!firstName || !lastName || !phone) {
            alert("يجب ملء جميع الحقول قبل الدخول.");
            return;
        }
        
        document.getElementById('step1').style.display = 'none';
        document.getElementById('step2').style.display = 'block';
    }

    function goToMainPage() {
        window.location.href = "https://sites.google.com/view/asahlak/%D8%A7%D9%84%D8%B5%D9%81%D8%AD%D9%87-%D8%A7%D9%84%D8%B1%D8%A6%D9%8A%D8%B3%D9%87";
    }
</script>

