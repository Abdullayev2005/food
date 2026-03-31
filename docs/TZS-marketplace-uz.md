# Texnik Topshiriq (TZS)

## Loyihaning nomi
**Xizmatlar va e’lonlar marketplace platformasi**

## 1. Loyiha maqsadi
Foydalanuvchilarga turli xizmatlar yoki e’lonlarni ko‘rish, qidirish, filterlash, aloqa qilish va administratorga e’lonlarni boshqarish imkonini beruvchi zamonaviy web-platforma yaratish.

Platforma quyidagilarni ta’minlashi kerak:
- e’lonlarni joylash
- e’lonlarni ko‘rish
- qidiruv va filter
- premium/VIP e’lonlar
- admin panel orqali boshqaruv
- mobil va desktop qurilmalarda qulay ishlash

---

## 2. Loyiha formati
Platforma:
- **web-sayt**
- keyinchalik **Telegram bot** yoki **mobil ilova** bilan integratsiya qilinishi mumkin

---

## 3. Foydalanuvchi rollari

### 3.1 Mehmon
- bosh sahifani ko‘rish
- e’lonlarni ko‘rish
- qidiruv qilish
- filterlash
- detail sahifaga kirish
- ro‘yxatdan o‘tish / login qilish

### 3.2 Ro‘yxatdan o‘tgan foydalanuvchi
- profil yaratish
- e’lon joylash
- o‘z e’lonlarini tahrirlash
- e’lonni o‘chirish
- premium/VIP qilish uchun so‘rov yuborish
- kelgan murojaatlar statistikasini ko‘rish

### 3.3 Administrator
- barcha e’lonlarni ko‘rish
- moderatsiya qilish
- tasdiqlash / rad etish
- kategoriyalarni boshqarish
- hududlarni boshqarish
- foydalanuvchilarni boshqarish
- premium/VIP belgilash
- banner/reklama bloklarini boshqarish
- platforma statistikasini ko‘rish

---

## 4. Asosiy funksional bo‘limlar

### 4.1 Bosh sahifa
Bosh sahifada quyidagilar bo‘lishi kerak:
- logo
- header
- qidiruv paneli
- kategoriyalar bloki
- VIP e’lonlar bloki
- eng yangi e’lonlar bloki
- hududlar bo‘yicha tezkor o‘tish
- footer

Bosh sahifa elementlari:
- Search input
- Category cards
- Top/VIP cards
- Recent listings grid
- CTA tugmalar:
  - E’lon joylash
  - Kategoriyalarni ko‘rish

### 4.2 Kategoriyalar sahifasi
Platformada e’lonlar kategoriyalar bo‘yicha ajratiladi.

Misol kategoriya turlari:
- Xizmatlar
- Ustalar
- Go‘zallik
- Ta’lim
- Ta’mirlash
- Transport
- Ijara
- Boshqalar

Har bir kategoriya uchun:
- nomi
- icon yoki rasm
- slug
- SEO title
- SEO description

### 4.3 Listing sahifasi
Bu sahifada ma’lum kategoriya yoki umumiy e’lonlar ro‘yxati chiqadi.

Funksiyalar:
- grid/list view
- pagination yoki infinite scroll
- sorting
- filterlash

Filterlar:
- kategoriya
- hudud/shahar
- narx oralig‘i
- sana
- VIP/oddiy
- reyting
- faqat rasmli e’lonlar

Sorting:
- eng yangi
- eng ko‘p ko‘rilgan
- narx bo‘yicha o‘sish
- narx bo‘yicha kamayish

### 4.4 E’lon detail sahifasi
Har bir e’lonning alohida sahifasi bo‘ladi.

Detail sahifada:
- sarlavha
- asosiy rasm
- rasm galereyasi
- to‘liq tavsif
- kategoriya
- hudud
- narx
- joylashtirilgan sana
- ko‘rishlar soni
- aloqa tugmalari
- muallif profili
- o‘xshash e’lonlar

Aloqa variantlari:
- telefon raqamni ko‘rsatish
- Telegram orqali yozish
- WhatsApp orqali yozish
- ichki forma orqali murojaat

### 4.5 E’lon joylash bo‘limi
Ro‘yxatdan o‘tgan foydalanuvchi yangi e’lon qo‘sha oladi.

Forma maydonlari:
- sarlavha
- qisqa tavsif
- to‘liq tavsif
- kategoriya
- subkategoriya
- hudud/shahar
- manzil
- narx
- telefon raqam
- Telegram username yoki link
- WhatsApp raqam
- rasm yuklash
- asosiy rasm tanlash

Validatsiya:
- majburiy maydonlar tekshiriladi
- telefon formati tekshiriladi
- rasm soni cheklanadi
- rasm hajmi cheklanadi
- nomaqbul so‘zlar filtrlanadi

### 4.6 Profil sahifasi
Ro‘yxatdan o‘tgan foydalanuvchi o‘z kabinetiga ega bo‘ladi.

Profil bo‘limlari:
- shaxsiy ma’lumotlar
- mening e’lonlarim
- e’lon holati
- VIP so‘rovlar
- balans yoki to‘lovlar tarixi
- parolni almashtirish

### 4.7 Admin panel
Admin panel alohida himoyalangan bo‘lim bo‘ladi.

Admin imkoniyatlari:
- dashboard
- foydalanuvchilar ro‘yxati
- e’lonlar ro‘yxati
- moderatsiya
- kategoriyalar
- hududlar
- reklamalar/bannerlar
- premium boshqaruvi
- statistikalar
- complaint/reportlar

Moderatsiya statuslari:
- draft
- pending
- approved
- rejected
- blocked
- archived

---

## 5. Moderatsiya logikasi
Har bir e’lon joylanganda:
1. foydalanuvchi formani to‘ldiradi
2. e’lon `pending` holatiga tushadi
3. admin tekshiradi
4. tasdiqlansa `approved`
5. rad qilinsa `rejected`

Avtomatik tekshiruv:
- taqiqlangan so‘zlar
- spamga o‘xshash sarlavha
- bir xil takroriy e’lonlar
- rasm sifati va hajmi
- noto‘g‘ri kategoriyalash

---

## 6. Premium/VIP tizimi
Platformada pullik ko‘tarish funksiyasi bo‘ladi.

VIP variantlar:
- Top listing
- Highlight rang
- Homepage’da chiqarish
- Kategoriyada tepaga chiqarish
- Muddatli premium status

Tariflar:
- 3 kun
- 7 kun
- 15 kun
- 30 kun

Admin paneldan qo‘lda yoki payment orqali avtomatik faollashadi.

---

## 7. Qidiruv tizimi
Qidiruv quyidagicha ishlashi kerak:
- sarlavha bo‘yicha
- tavsif bo‘yicha
- kategoriya bo‘yicha
- hudud bo‘yicha

Qo‘shimcha:
- typo tolerant search
- takliflar chiqishi
- recent searches
- popular queries

---

## 8. Statistikalar
Har bir e’lon uchun:
- ko‘rishlar soni
- aloqa tugmasi bosilgan soni
- telefon ochilgan soni
- Telegram bosilgan soni

Admin uchun:
- jami foydalanuvchilar
- jami e’lonlar
- bugungi yangi e’lonlar
- tasdiqlangan e’lonlar
- premium e’lonlar soni
- eng faol kategoriya
- eng faol hudud

---

## 9. Dizayn talablari
Umumiy stil:
- zamonaviy
- minimalistik
- tez yuklanadigan
- mobil-first
- premium ko‘rinish

Rang sxemasi:
- oq / qora / aksent rang, yoki
- qoramtir premium theme

UI elementlar:
- katta qidiruv paneli
- aniq CTA tugmalar
- card-based layout
- soft shadow
- rounded corners
- skeleton loader

---

## 10. Texnik stack
Frontend:
- **Next.js**
- **Tailwind CSS**
- **TypeScript**
- **React Hook Form**
- **Zod**
- **TanStack Query**

Backend:
- **Node.js / Next.js API** yoki **NestJS**

Database:
- **PostgreSQL**

ORM:
- **Prisma**

Storage:
- **Cloudinary** yoki **Supabase Storage** yoki **AWS S3**

Auth:
- JWT yoki NextAuth yoki Supabase Auth

---

## 11. Database struktura

### users
- id
- full_name
- phone
- email
- password_hash
- telegram_username
- role
- status
- created_at
- updated_at

### categories
- id
- name
- slug
- icon
- parent_id
- is_active
- created_at

### regions
- id
- name
- slug
- is_active

### listings
- id
- user_id
- category_id
- region_id
- title
- short_description
- description
- price
- currency
- address
- phone
- telegram_link
- whatsapp
- status
- is_vip
- vip_expire_at
- views_count
- created_at
- updated_at

### listing_images
- id
- listing_id
- image_url
- is_main
- sort_order

### reports
- id
- listing_id
- user_id
- reason
- status
- created_at

### payments
- id
- user_id
- listing_id
- amount
- currency
- payment_method
- status
- created_at

### contact_clicks
- id
- listing_id
- click_type
- user_ip
- created_at

---

## 12. API bo‘limlari

Auth API:
- POST `/api/auth/register`
- POST `/api/auth/login`
- POST `/api/auth/logout`
- GET `/api/auth/me`

Listing API:
- GET `/api/listings`
- GET `/api/listings/:id`
- POST `/api/listings`
- PATCH `/api/listings/:id`
- DELETE `/api/listings/:id`

Category API:
- GET `/api/categories`

Region API:
- GET `/api/regions`

Admin API:
- GET `/api/admin/listings`
- PATCH `/api/admin/listings/:id/status`
- GET `/api/admin/users`
- PATCH `/api/admin/users/:id`
- POST `/api/admin/categories`
- PATCH `/api/admin/categories/:id`

Payment API:
- POST `/api/payments/create`
- POST `/api/payments/webhook`

---

## 13. Xavfsizlik talablari
- parollar hash bo‘lib saqlanishi kerak
- admin route’lar himoyalangan bo‘lishi kerak
- rate limiting bo‘lishi kerak
- spamdan himoya
- CSRF/XSS/SQL injectiondan himoya
- rasm yuklashda file validation
- audit log yuritilishi kerak

---

## 14. SEO talablari
- har bir kategoriya uchun unique meta title
- har bir listing uchun SEO slug
- sitemap.xml
- robots.txt
- Open Graph image
- structured data
- canonical link
- pagination SEO

---

## 15. Performance talablari
- sahifa yuklanishi tez bo‘lishi kerak
- rasmlar optimizatsiya qilinishi kerak
- lazy loading ishlashi kerak
- server response minimal kechikish bilan bo‘lishi kerak
- caching qo‘llanilishi kerak

---

## 16. Responsive talablari
Platforma quyidagi ekranlarga mos bo‘lishi kerak:
- mobil
- planshet
- desktop

Mobil uchun:
- bottom CTA
- compact filter
- swipe gallery
- sticky contact button

---

## 17. Qo‘shimcha funksiyalar
- favoritga saqlash
- shikoyat qilish
- e’lonni ulashish
- ko‘rilgan e’lonlar tarixi
- push notification
- email notification
- Telegram notification
- admin activity log

---

## 18. To‘lov tizimi
Agar monetizatsiya bo‘lsa:
- Click
- Payme
- Uzum Bank
- Stripe (keyinchalik)

To‘lov scenariysi:
1. foydalanuvchi VIP tanlaydi
2. tarif tanlaydi
3. to‘lov qiladi
4. tizim statusni yangilaydi
5. e’lon premium holatga o‘tadi

---

## 19. Ish jarayoni bosqichlari
1-bosqich:
- talablarni yig‘ish
- dizayn prototip
- DB schema
- texnik arxitektura

2-bosqich:
- frontend layout
- auth
- listing CRUD
- admin panel boshlang‘ich

3-bosqich:
- filter
- qidiruv
- SEO
- premium logika

4-bosqich:
- test
- optimizatsiya
- deploy
- monitoring

---

## 20. Testlash
Test turlari:
- functional test
- UI test
- responsive test
- API test
- admin panel test
- form validation test
- payment test
- security test

---

## 21. Deploy
Tavsiya:
- Frontend: Vercel
- Backend: VPS / Railway / Render
- Database: Neon / Supabase / Railway PostgreSQL
- Storage: Cloudinary

---

## 22. Kelajakdagi kengaytirishlar
- Telegram bot integratsiya
- mobil ilova
- chat tizimi
- ichki balans
- promo kod
- referral system
- AI moderatsiya
- auto-tagging
- tavsiya algoritmi

---

## Foydalanuvchi oqimi

### Mehmon oqimi
1. saytga kiradi
2. qidiruv qiladi
3. e’lonni ochadi
4. aloqa qiladi
5. ro‘yxatdan o‘tishga qaror qiladi

### E’lon beruvchi oqimi
1. login qiladi
2. e’lon joylaydi
3. moderatsiyaga tushadi
4. tasdiqlanadi
5. VIP qiladi
6. murojaatlar oladi

### Admin oqimi
1. panelga kiradi
2. pending e’lonlarni ko‘radi
3. tekshiradi
4. approve/reject qiladi
5. statistika ko‘radi

---

## Minimal MVP
- Home page
- Listing page
- Detail page
- Login/Register
- Add listing form
- User profile
- Admin moderation
- Search
- Basic filters

## To‘liq versiya
- premium
- payment
- analytics
- report system
- favorites
- recommendation
- SEO advanced
- notification system
