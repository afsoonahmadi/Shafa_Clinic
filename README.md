<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>درمانگاه شبانه روزی شفا</title>
  <style>
    /* Reset و استایل پایه */
    body {
      font-family: Tahoma, sans-serif;
      background: #f9f9f9;
      margin: 0;
      padding: 0;
      color: #333;
    }
    header {
      background-color: #2c3e50;
      color: white;
      padding: 15px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      font-size: 1.6rem;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 15px;
      font-weight: bold;
    }
    nav a:hover {
      text-decoration: underline;
    }
    main {
      max-width: 900px;
      margin: 20px auto;
      padding: 0 20px;
    }
    section {
      background: white;
      border-radius: 8px;
      padding: 20px;
      margin-bottom: 25px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
    }
    h2 {
      margin-top: 0;
      color: #34495e;
      border-bottom: 2px solid #2980b9;
      padding-bottom: 6px;
    }
    ul.services-list {
      list-style: none;
      padding: 0;
    }
    ul.services-list li {
      padding: 8px 0;
      border-bottom: 1px solid #eee;
    }
    ul.doctors-list {
      list-style: none;
      padding: 0;
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
    }
    ul.doctors-list li {
      border: 1px solid #ddd;
      padding: 15px;
      border-radius: 8px;
      width: calc(50% - 15px);
      box-sizing: border-box;
      background: #fefefe;
    }
    ul.doctors-list img {
      width: 80px;
      height: 80px;
      border-radius: 50%;
      object-fit: cover;
      margin-bottom: 10px;
    }
    form label {
      display: block;
      margin-top: 12px;
      font-weight: bold;
    }
    form input, form select, form textarea {
      width: 100%;
      padding: 8px;
      margin-top: 5px;
      border: 1px solid #ccc;
      border-radius: 5px;
      box-sizing: border-box;
      font-size: 1rem;
      font-family: inherit;
      resize: vertical;
    }
    form button {
      margin-top: 15px;
      padding: 10px 15px;
      background-color: #2980b9;
      border: none;
      color: white;
      font-weight: bold;
      cursor: pointer;
      border-radius: 5px;
      transition: background-color 0.3s ease;
    }
    form button:hover {
      background-color: #1c5980;
    }
    footer {
      text-align: center;
      padding: 15px 10px;
      font-size: 0.9rem;
      color: #777;
      background: #f0f0f0;
      margin-top: 40px;
    }
    .lang-switch {
      cursor: pointer;
      font-weight: bold;
    }
  </style>
</head>
<body>

<header>
  <h1>درمانگاه شبانه روزی شفا</h1>
  <nav>
    <a href="#services">خدمات</a>
    <a href="#doctors">پزشکان</a>
    <a href="#appointment">نوبت دهی</a>
    <span class="lang-switch" id="langSwitch">English</span>
  </nav>
</header>

<main>

  <section id="intro">
    <h2>خوش آمدید</h2>
    <p>
      درمانگاه شبانه روزی شفا در سیرجان واقع شده است.<br/>
      آدرس: سیرجان - چهارراه موحدی - جنب داروخانه آریا<br/>
      شماره تماس: ۰۳۴۴۲۲۷۲۲۴۵<br/>
      ساعت کاری: شبانه روزی
    </p>
  </section>

  <section id="services">
    <h2>خدمات ما</h2>
    <ul class="services-list">
      <li>پزشک عمومی و متخصص</li>
      <li>تزریقات</li>
      <li>دندانپزشکی</li>
      <li>مامایی</li>
      <li>روانشناسی</li>
      <li>تخصص‌های داخلی، اطفال، نوروسرجری، قلب</li>
    </ul>
  </section>

  <section id="doctors">
    <h2>پزشکان ما</h2>
    <ul class="doctors-list">
      <li>
        <img src="https://via.placeholder.com/80" alt="دکتر علی رضایی" />
        <strong>دکتر علی رضایی</strong><br/>
        متخصص داخلی
      </li>
      <li>
        <img src="https://via.placeholder.com/80" alt="دکتر مریم حسینی" />
        <strong>دکتر مریم حسینی</strong><br/>
        متخصص اطفال
      </li>
      <li>
        <img src="https://via.placeholder.com/80" alt="دکتر ناصر محمدی" />
        <strong>دکتر ناصر محمدی</strong><br/>
        نوروسرجری
      </li>
      <li>
        <img src="https://via.placeholder.com/80" alt="دکتر سارا کریمی" />
        <strong>دکتر سارا کریمی</strong><br/>
        متخصص قلب
      </li>
    </ul>
  </section>

  <section id="appointment">
    <h2>نوبت دهی آنلاین</h2>
    <form id="appointmentForm">
      <label for="fullname">نام و نام خانوادگی:</label>
      <input type="text" id="fullname" name="fullname" required />

      <label for="phone">شماره تماس:</label>
      <input type="tel" id="phone" name="phone" required pattern="^\d{10,11}$" placeholder="مثال: 09123456789" />

      <label for="specialty">تخصص مورد نظر:</label>
      <select id="specialty" name="specialty" required>
        <option value="">انتخاب تخصص</option>
        <option value="general">پزشک عمومی و متخصص</option>
        <option value="interna">داخلی</option>
        <option value="pediatrics">اطفال</option>
        <option value="neurosurgery">نوروسرجری</option>
        <option value="cardiology">قلب</option>
        <option value="dentistry">دندانپزشکی</option>
        <option value="midwifery">مامایی</option>
        <option value="psychology">روانشناسی</option>
      </select>

      <label for="doctor">انتخاب پزشک:</label>
      <select id="doctor" name="doctor" required>
        <option value="">ابتدا تخصص را انتخاب کنید</option>
      </select>

      <label for="date">تاریخ نوبت:</label>
      <input type="date" id="date" name="date" required min="" />

      <label for="time">ساعت نوبت:</label>
      <input type="time" id="time" name="time" required />

      <label for="notes">توضیحات (اختیاری):</label>
      <textarea id="notes" name="notes" rows="3"></textarea>

      <button type="submit">ثبت نوبت</button>
    </form>
    <div id="formMessage" style="margin-top:15px;color:green;"></div>
  </section>

</main>

<footer>
  © 2025 درمانگاه شبانه روزی شفا - آدرس: سیرجان، چهارراه موحدی، جنب داروخانه آریا - تلفن: ۰۳۴۴۲۲۷۲۲۴۵
</footer>

<script>
  // تنظیم حداقل تاریخ برای انتخاب تاریخ نوبت (از امروز)
  const dateInput = document.getElementById('date');
  const today = new Date().toISOString().split('T')[0];
  dateInput.min = today;

  // پزشکان بر اساس تخصص
  const doctorsBySpecialty = {
    general: [
      { id: 'ali_rezaei', name: 'دکتر علی رضایی' },
      { id: 'maryam_hosseini', name: 'دکتر مریم حسینی' }
    ],
    interna: [
      { id: 'ali_rezaei', name: 'دکتر علی رضایی' }
    ],
    pediatrics: [
      { id: 'maryam_hosseini', name: 'دکتر مریم حسینی' }
    ],
    neurosurgery: [
      { id: 'naser_mohammadi', name: 'دکتر ناصر محمدی' }
    ],
    cardiology: [
      { id: 'sara_karimi', name: 'دکتر سارا کریمی' }
    ],
    dentistry: [
      { id: 'dentist_placeholder', name: 'دندانپزشک' }
    ],
    midwifery: [
      { id: 'midwife_placeholder', name: 'مامایی' }
    ],
    psychology: [
      { id: 'psychologist_placeholder', name: 'روانشناس' }
    ]
  };

  const specialtySelect = document.getElementById('specialty');
  const doctorSelect = document.getElementById('doctor');

  specialtySelect.addEventListener('change', () => {
    const specialty = specialtySelect.value;
    doctorSelect.innerHTML = '';

    if (!specialty || !doctorsBySpecialty[specialty]) {
      doctorSelect.innerHTML = '<option value="">ابتدا تخصص را انتخاب کنید</option>';
      return;
    }

    const options = doctorsBySpecialty[specialty]
      .map(doc => `<option value="${doc.id}">${doc.name}</option>`)
      .join('');
    doctorSelect.innerHTML = options;
  });

  // فرم نوبت دهی: فقط نمایش پیام تایید (بدون ارسال به سرور)
  const form = document.getElementById('appointmentForm');
  const formMessage = document.getElementById('formMessage');

  form.addEventListener('submit', (e) => {
    e.preventDefault();

    // دریافت اطلاعات فرم (می‌تونید اینجا ارسال به سرور رو اضافه کنید)
    const fullname = form.fullname.value.trim();
    const phone = form.phone.value.trim();
    const specialty = form.specialty.options[form.specialty.selectedIndex].text;
    const doctor = form.doctor.options[form.doctor.selectedIndex].text;
    const date = form.date.value;
    const time = form.time.value;

    formMessage.style.color = 'green';
    formMessage.textContent = `نوبت شما برای ${fullname} با ${doctor} در تخصص ${specialty}، تاریخ ${date} ساعت ${time} ثبت شد. با شما تماس گرفته خواهد شد.`;

    form.reset();
    doctorSelect.innerHTML = '<option value="">ابتدا تخصص را انتخاب کنید</option>';
  });

  // سوئیچ زبان (فارسی - انگلیسی) - فقط متن نمونه
  const langSwitch = document.getElementById('langSwitch');
  let isPersian = true;

  langSwitch.addEventListener('click', () => {
    if (isPersian) {
      document.documentElement.lang = 'en';
      document.documentElement.dir = 'ltr';
      document.body.style.fontFamily = 'Arial, sans-serif';

      document.querySelector('header h1').textContent = 'Shafa 24-Hour Clinic';
      document.querySelector('nav').innerHTML = `
        <a href="#services">Services</a>
        <a href="#doctors">Doctors</a>
        <a href="#appointment">Appointment</a>
        <span class="lang-switch" id="langSwitch">فارسی</span>
      `;

      document.getElementById('intro').innerHTML = `
        <h2>Welcome</h2>
        <p>
          Shafa 24-Hour Clinic is located in Sirjan.<br/>
          Address: Sirjan - Moahidi Crossroad - Next to Aria Pharmacy<br/>
          Phone: 03442272245<br/>
          Working Hours: 24/7
        </p>
      `;

      document.getElementById('services').innerHTML = `
        <h2>Our Services</h2>
        <ul class="services-list">
          <li>General and Specialist Physicians</li>
          <li>Injections</li>
          <li>Dentistry</li>
          <li>Midwifery</li>
          <li>Psychology</li>
          <li>Internal Medicine, Pediatrics, Neurosurgery, Cardiology</li>
        </ul>
      `;

      document.getElementById('doctors').innerHTML = `
        <h2>Our Doctors</h2>
        <ul class="doctors-list">
          <li>
            <img src="https://via.placeholder.com/80" alt="Dr. Ali Rezaei" />
            <strong>Dr. Ali Rezaei</strong><br/>
            Internal Medicine Specialist
          </li>
          <li>
            <img src="https://via.placeholder.com/80" alt="Dr. Maryam Hosseini" />
            <strong>Dr. Maryam Hosseini</strong><br/>
            Pediatrics Specialist
          </li>
          <li>
            <img src="https://via.placeholder.com/80" alt="Dr. Naser Mohammadi" />
            <strong>Dr. Naser Mohammadi</strong><br/>
            Neurosurgery
          </li>
          <li>
            <img src="https://via.placeholder.com/80" alt="Dr. Sara Karimi" />
            <strong>Dr. Sara Karimi</strong><br/>
            Cardiology Specialist
          </li>
        </ul>
      `;

      document.getElementById('appointment').innerHTML = `
        <h2>Online Appointment</h2>
        <form id="appointmentForm">
          <label for="fullname">Full Name:</label>
          <input type="text" id="fullname" name="fullname" required />

          <label for="phone">Phone Number:</label>
          <input type="tel" id="phone" name="phone" required placeholder="Example: +1234567890" />

          <label for="specialty">Choose Specialty:</label>
          <select id="specialty" name="specialty" required>
            <option value="">Select Specialty</option>
            <option value="general">General and Specialist Physicians</option>
            <option value="interna">Internal Medicine</option>
            <option value="pediatrics">Pediatrics</option>
            <option value="neurosurgery">Neurosurgery</option>
            <option value="cardiology">Cardiology</option>
            <option value="dentistry">Dentistry</option>
            <option value="midwifery">Midwifery</option>
            <option value="psychology">Psychology</option>
          </select>

          <label for="doctor">Choose Doctor:</label>
          <select id="doctor" name="doctor" required>
            <option value="">Select specialty first</option>
          </select>

          <label for="date">Appointment Date:</label>
          <input type="date" id="date" name="date" required min="${today}" />

          <label for="time">Appointment Time:</label>
          <input type="time" id="time" name="time" required />

          <label for="notes">Notes (Optional):</label>
          <textarea id="notes" name="notes" rows="3"></textarea>

          <button type="submit">Submit Appointment</button>
        </form>
        <div id="formMessage" style="margin-top:15px;color:green;"></div>
      `;

      // دوباره المان‌ها را تعریف کنیم
      attachFormEvents();

      isPersian = false;
    } else {
      location.reload();
    }
  });

  function attachFormEvents() {
    const specialtySelect = document.getElementById('specialty');
    const doctorSelect = document.getElementById('doctor');
    const form = document.getElementById('appointmentForm');
    const formMessage = document.getElementById('formMessage');

    specialtySelect.addEventListener('change', () => {
      const specialty = specialtySelect.value;
      doctorSelect.innerHTML = '';

      if (!specialty || !doctorsBySpecialty[specialty]) {
        doctorSelect.innerHTML = '<option value="">' + (document.documentElement.lang === 'fa' ? 'ابتدا تخصص را انتخاب کنید' : 'Select specialty first') + '</option>';
        return;
      }

      const options = doctorsBySpecialty[specialty]
        .map(doc => `<option value="${doc.id}">${doc.name}</option>`)
        .join('');
      doctorSelect.innerHTML = options;
    });

    form.addEventListener('submit', (e) => {
      e.preventDefault();

      const fullname = form.fullname.value.trim();
      const phone = form.phone.value.trim();
      const specialty = specialtySelect.options[specialtySelect.selectedIndex].text;
      const doctor = doctorSelect.options[doctorSelect.selectedIndex].text;
      const date = form.date.value;
      const time = form.time.value;

      formMessage.style.color = 'green';
      if(document.documentElement.lang === 'fa'){
        formMessage.textContent = `نوبت شما برای ${fullname} با ${doctor} در تخصص ${specialty}، تاریخ ${date} ساعت ${time} ثبت شد. با شما تماس گرفته خواهد شد.`;
      } else {
        formMessage.textContent = `Your appointment for ${fullname} with ${doctor} in specialty ${specialty} on ${date} at ${time} has been booked. We will contact you soon.`;
      }

      form.reset();
      doctorSelect.innerHTML = '<option value="">' + (document.documentElement.lang === 'fa' ? 'ابتدا تخصص را انتخاب کنید' : 'Select specialty first') + '</option>';
    });
  }

  attachFormEvents();

</script>

</body>
</html>
