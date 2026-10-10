MANA VELUGU DIGITAL MEDIA — NEW WEBSITE FILES

ఫైళ్లు:
1. index.html — పబ్లిక్ న్యూస్ వెబ్‌సైట్
2. admin.html — అడ్మిన్ లాగిన్, వార్తలు ప్రచురించడం/దాచడం/తొలగించడం
3. config.js — Supabase కనెక్షన్ వివరాలు ఇక్కడ పెట్టాలి
4. setup_news.sql — కొత్త Supabase project లో SQL Editor ద్వారా ఒక్కసారి Run చేయాలి

గమనిక: ఈ ఫైళ్లు కొత్త సైట్‌కు starter package. Supabase project, database, admin auth user, Vercel deployment సెట్ చేసిన తర్వాతే live site పూర్తిగా పనిచేస్తుంది.

సెటప్ క్రమం:
1. కొత్త Supabase project సృష్టించండి.
2. SQL Editor లో setup_news.sql మొత్తం paste చేసి Run చేయండి.
3. Authentication > Users లో కొత్త admin user సృష్టించండి. Signup public గా enable చేయకండి.
4. Project Settings > API (లేదా API Keys) లో Project URL మరియు Publishable key/anon key తీసుకోండి.
5. config.js లో PASTE_NEW_SUPABASE_PROJECT_URL_HERE మరియు PASTE_NEW_SUPABASE_PUBLISHABLE_OR_ANON_KEY_HERE స్థానాల్లో మీ వివరాలు పెట్టండి. service_role/secret key వాడకండి.
6. ఈ నాలుగు ఫైళ్లను కొత్త GitHub repository root లో upload చేయండి.
7. Vercel లో కొత్త project గా ఆ repository ని import/deploy చేయండి.
8. Public URL లో index.html తెరవండి; Admin కోసం అదే domain లో /admin.html తెరవండి.

సెక్యూరిటీ: ఈ starter policy లో authenticated Supabase users కు admin చర్యలు అనుమతిస్తాయి. Supabase project-இல் admin account மட்டும் வைத்திருக்கவும்; வேறு authenticated users உருவாக்க வேண்டாம். production பாதுகாப்பு தேவைக்கு admin_users table மூலம் admin-only policies சேர்க்கலாம்.

இந்த அமைப்பில் PDF/ePaper feature இல்லை.
