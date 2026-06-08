# NaijaHub — Deployment Checklist

## Critical Fixes
- UUID consistency fixed (auth.users alignment)
- Wallet upsert race condition fixed
- Auth trigger auto-creates profiles
- Premium subscriptions unique constraint added
- Realtime chat improvements applied

## Supabase Setup
1. Run migrations in SQL editor
2. Create storage bucket: naijahub-uploads
3. Enable RLS on all tables

## Netlify Setup
- Build command: npm run build
- Plugin: @netlify/plugin-nextjs

## Environment Variables
- NEXT_PUBLIC_SUPABASE_URL
- NEXT_PUBLIC_SUPABASE_ANON_KEY
- SUPABASE_SERVICE_ROLE_KEY
- PAYSTACK_SECRET_KEY

## Deployment
1. Push to GitHub
2. Netlify auto deploy
3. Configure Supabase auth redirects

## Notes
Ensure RLS policies are tested before production.
