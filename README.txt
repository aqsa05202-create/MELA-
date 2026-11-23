Mela v3 - Google Login GitHub Pages redirect fix

1. Upload/replace index.html at the root of the GitHub Pages repository for:
   https://aqsa05202-create.github.io/MELE/

2. Supabase Dashboard > Authentication > URL Configuration:
   Site URL:
   https://aqsa05202-create.github.io/MELE/

   Add these Redirect URLs:
   https://aqsa05202-create.github.io/MELE/
   https://aqsa05202-create.github.io/MELE/**

3. Supabase > Authentication > Sign In / Providers > Google:
   Keep Google enabled. Client ID and Client Secret must both be set.
   Never put the Google Client Secret in index.html or any public repository.

4. Test by opening the live GitHub Pages URL (not localhost) and using Continue with Google.
   This build explicitly sends the OAuth callback back to the live Mela URL.
