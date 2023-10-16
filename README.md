# hotspot_captive_portal
Android Hotspot Captive Portal 
# common issue fix
আপনি যদি php সার্ভার লোকাল hoste ফাইলগুলো রান করেন : <code> php -S 127.0.0.0:8080 </code> তাহলে আপনি একটি সমস্যার সম্মুখীন হবেন যখন ইউজার সেখানে তাদের তথ্য সাবমিট করবে। 
![Screenshot_2023-10-16-16-13-40-261_idm internet download manager plus](https://github.com/masshuvo/hotspot_captive_portal/assets/108648096/f812109a-67e2-4f14-8d6e-7428225eb2ec)

#solution
অবশ্যই আপনার সম্পূর্ণ ফাইলগুলোর পারমিশন দেখে নিবেন। 
মূলত ফাইলগুলোর পারমিশন যদি এরকম থাকে:

![Screenshot_2023-10-16-16-13-17-704_com termux](https://github.com/masshuvo/hotspot_captive_portal/assets/108648096/faf9b2fa-79fb-488d-bba3-e8a05ed86b9e)

তাহলেই উপরের দেখানো স্ক্রিনশটের সমস্যাটি দেখাবে।
<code> chmod o+w * </code> এই কোডটি এক্সিকিউট করার মাধ্যমে ফাইলগুলো পারমিশন পরিবর্তন হবে: 
![Screenshot_2023-10-16-16-12-55-634_com termux](https://github.com/masshuvo/hotspot_captive_portal/assets/108648096/9a76bf43-a902-484b-a25b-2376f5ab97fc)

এখন ঠিকভাবে রান করবে।
