# Gentoo setup for ASUS UX410UAR

Because of LVM and LUKS, I am using `genkernel`:


    sudo cp git/gentoo-asus-ux410uar/usr/src/linux/.config /usr/src/linux/
    time sudo genkernel --makeopts=-j11 --menuconfig --lvm --luks all
    sudo grub-mkconfig -o /boot/grub/grub.cfg


