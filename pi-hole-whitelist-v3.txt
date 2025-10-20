# 🇹🇭 Pi-hole Whitelist (Thailand Edition)
# ------------------------------------
# Maintainer: 7MannSo
# Version: 2025-10-v3
# Description:
#   Common whitelist domains for Thai users — designed for Pi-hole use.
#   Includes popular social, shopping, banking, media, and education domains.
#   Ideal for home, café, or small business Pi-hole installations.
# ------------------------------------

# ====================================
# 🟦 SOCIAL MEDIA & COMMUNICATION
# ====================================
# Allow major communication & social platforms to function properly.

facebook.com
fbcdn.com
fbsbx.com
facebook.net
instagram.com
cdninstagram.com
threads.net
messenger.com
meta.com
whatsapp.com
whatsapp.net

line.me
line-apps.com
linecorp.com
linecdn.net
line-scdn.net
linew.me
linetv.tw
today.line.me
shopping.line.me
uts-front.line-apps.com

x.com
twitter.com
t.co
twimg.com
api.twitter.com
abs.twimg.com
pbs.twimg.com
video.twimg.com
ton.twimg.com

telegram.org
t.me
discord.com
cdn.discordapp.com
zoom.us

# ====================================
# 🛍️ SHOPPING & E-COMMERCE
# ====================================
# Whitelist for major e-commerce platforms used in Thailand.

# --- Shopee / LINE Shopping ---
shopee.co.th
shopeemobile.com
cf.shopee.co.th
api.shopee.co.th
uts-front.line-apps.com

# --- Lazada ---
lazada.co.th
my.lazada.co.th
s.lazada.co.th
icms.lazada.co.th
laz-img-cdn.alicdn.com
alicdn.com
alibaba.com
alipay.com
lazglobal.com
assets.alicdn.com
lazada.sg

# --- JD Central ---
jd.co.th
jdth.com
jdcdn.com

# ====================================
# 💳 BANKING / CREDIT / FINANCE (TH)
# ====================================
# Whitelist for Thai banking, credit cards, and finance apps.

bbl.co.th
bangkokbank.com

ktb.co.th
krungthai.com

scb.co.th
scbapi.scb.co.th

kbank.co.th
kasikornbank.com

krungsri.com
krungsrionline.com
krungsricard.com
mobile.servicekrungsrigroup.com
www.krungsrimobile.com

gsb.or.th

ttbbank.com
tmbbank.com

ghb.co.th

promptpay.io
npay.or.th
ndid.or.th
govwallet.go.th

aeon.co.th
aeonnetservice.com
aeonmicrofinance.com
aeoncredit.co.th

umayplus.co.th
easybuy.co.th
umayplus.com
ebm.co.th

# ====================================
# 🎓 EDUCATION / UNIVERSITIES (TH)
# ====================================
# Common domains for major Thai universities.
# Helps avoid blocking academic and e-learning services.

chula.ac.th
cu.ac.th
mahidol.ac.th
kku.ac.th
ku.ac.th
cmu.ac.th
psu.ac.th
bu.ac.th
su.ac.th
wu.ac.th
spu.ac.th
mut.ac.th
rmutp.ac.th
rmuti.ac.th
rmutk.ac.th
rmutl.ac.th
rmutr.ac.th
rmutto.ac.th
npru.ac.th
mfu.ac.th
kmutt.ac.th
kmitl.ac.th
nu.ac.th
swu.ac.th
tni.ac.th
tu.ac.th
au.edu
stamford.edu
buu.ac.th
utcc.ac.th
dpu.ac.th
msu.ac.th
phuket.psu.ac.th
ubu.ac.th
pim.ac.th
rsu.ac.th

# ====================================
# 🎬 STREAMING & MEDIA
# ====================================
youtube.com
ytimg.com
googlevideo.com
netflix.com
nflxvideo.net
nflximg.net
spotify.com
scdn.co
joox.com
jooxcdn.com

# ====================================
# 🧭 TRAVEL / MAP / SERVICE
# ====================================
grab.com
grbcdn.net
food.grab.com
mapbox.com
maps.googleapis.com
googlemaps.com
booking.com
agoda.com
traveloka.com
airasia.com

# ====================================
# 💬 CLOUD / CDN / API
# ====================================
amazonaws.com
cloudfront.net
akamai.net
akamaized.net
googleusercontent.com
firebaseio.com
fastly.net
cdn77.org

# ====================================
# 📱 SYSTEM SERVICES (GOOGLE / APPLE / MICROSOFT)
# ====================================
google.com
gstatic.com
googleapis.com
ggpht.com
play.google.com
android.clients.google.com
apple.com
icloud.com
mzstatic.com
apps.apple.com
live.com
microsoft.com
office.com
onenote.com
teams.microsoft.com

# ====================================
# 🏛️ GOVERNMENT / UTILITIES (TH)
# ====================================
go.th
thaigov.go.th
mof.go.th
egat.co.th
mea.or.th
pea.co.th

# ====================================
# ✅ Notes
# - Maintained by: 7MannSo (https://github.com/7MannSo)
# - Check Pi-hole Query Log regularly to fine-tune allowed domains.
# - Import command:
#     sudo pihole -w $(cat pi-hole-whitelist-full.txt | grep -v '^#')
# - Recommended to review every 3 months for CDN/domain updates.
# ====================================
