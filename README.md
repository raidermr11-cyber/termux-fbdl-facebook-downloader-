# termux-fbdl-facebook-downloader-
Termux-এ Facebook Video &amp; Reels ডাউনলোডার স্ক্রিপ্ট
# Termux Facebook Video Downloader (fbdl)

একদম সহজ Facebook Reels ও ভিডিও ডাউনলোডার Termux-এর জন্য।  
Facebook অ্যাপ থেকে Share → Termux → কোয়ালিটি সিলেক্ট → ডাউনলোড!

Termux-এ যা যা ইনস্টল করতে হবে (একবারই করবে)
Termux অ্যাপ খুলে নিচের সব কমান্ড একে একে চালাও (প্রত্যেকটা শেষ হওয়ার পর Enter চাপো):
# ১. Termux আপডেট করো
pkg update && pkg upgrade -y

# ২. স্টোরেজ অ্যাক্সেস দাও (Download ফোল্ডারে সেভ করার জন্য)
termux-setup-storage

# ৩. প্রয়োজনীয় প্যাকেজ ইনস্টল করো
pkg install python git ffmpeg -y

# ৪. yt-dlp ইনস্টল/আপডেট করো (এটাই মূল টুল)
pip install -U yt-dlp
শেষ হয়ে গেলে এই কমান্ডটা চালিয়ে চেক করো যে সব ঠিক আছে কি না:
yt-dlp --version
যদি ভার্সন দেখায় (যেমন: 2026.xx.xx), তাহলে ঠিক আছে।
এখন তোমার fbdl স্ক্রিপ্ট সেটআপ করো
cd \~
git clone https://github.com/raidermr11-cyber/termux-fbdl.git
cd termux-fbdl

# স্ক্রিপ্টকে Termux-এর শেয়ার সিস্টেমে কপি করো
cp fbdl \~/.termux/termux-url-opener
chmod +x \~/.termux/termux-url-opener
