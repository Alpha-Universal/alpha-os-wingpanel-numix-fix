# alpha-os-wingpanel-numix-fix

As of this writing (November 2017), installing Numix or Numix-Circle to Pantheon in elementary OS Loki replaces the upper-right Wingpanel icons with oversized Numix equivalents, and shows numerous missing icons throughout many applications.  

The fix entails modifying the inherits rule in Numix's index.theme file, deleting all Numix/scalable/status icons, and deleting both system-shutdown-symbolic.svg icons in Numix{-Light}/scalable/actions.  Those changes force elementary icons to in Wingpanel's upper-right, replace missing Numix icons with elementary ones, and use Numix icons everywhere else.

The contents of this repo simply mirror the stable releases of Numix and Numix-Circle, so those icon files won't be hosted.  Instead, the deb with the above changes implemented and its debian packaging files are hosted for those who don't want to enable the alpha repository (instructions here for those who do: https://alpha.store/forums/topic/alpha-software-repo-now-available/) to pull updates through apt.  
