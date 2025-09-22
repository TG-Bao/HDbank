# 🚨 QUICK SETUP - Sửa lỗi ngay!

## Lỗi hiện tại:
```
Error: Invalid supabaseUrl: Must be a valid HTTP or HTTPS URL.
```

## Giải pháp:

### Bước 1: Cập nhật file `.env.local`
Mở file `.env.local` và thay thế các giá trị sau:

```env
# Thay thế dòng này:
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url

# Bằng URL thực tế của bạn, ví dụ:
NEXT_PUBLIC_SUPABASE_URL=https://abcdefghijklmnop.supabase.co
```

### Bước 2: Lấy thông tin Supabase
1. Vào [Supabase Dashboard](https://supabase.com/dashboard)
2. Chọn project của bạn
3. Vào **Settings** > **API**
4. Copy các giá trị:
   - **Project URL** → `NEXT_PUBLIC_SUPABASE_URL`
   - **anon public** key → `NEXT_PUBLIC_SUPABASE_ANON_KEY`
   - **service_role** key → `SUPABASE_SERVICE_ROLE_KEY`

### Bước 3: Chạy lại
```bash
npm run dev
```

## Ví dụ file .env.local hoàn chỉnh:
```env
NEXT_PUBLIC_SUPABASE_URL=https://abcdefghijklmnop.supabase.co
NEXT_PUBLIC_SUPABASE_ANON_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
SUPABASE_SERVICE_ROLE_KEY=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
OPENAI_API_KEY=your_openai_api_key_here
NEXT_PUBLIC_APP_URL=http://localhost:3000
```

## ✅ Sau khi sửa xong:
- Chạy `npm run dev`
- Truy cập http://localhost:3000
- Đăng ký tài khoản
- Vào Admin Panel để upload tài liệu
