
classe = input('Qual a classe de IP[A, B, C]:').upper()
ma = int(input('Digite a quantidade de máquinas: '))

qm = (2, 4, 8, 16, 32, 64, 128, 256)
ma2 = 0
bit = 0
if classe == 'C':
    print()
    for a in (qm):
        bit = bit + 1
        if a >= (ma + 2) and (ma < 255):
            ma2 = 256 - a
            print('Mascara da rede: \033[0;0;34m255.255.255.{}\033[m'.format(ma2))
            if ma == 0:
                bit = bit - 1
            break

    if ma >= 255 and ma <= 65534:
        bit = 8
        ma2 = ma / 256
        for a2 in (qm):
            bit = bit + 1
            if (a2 * 256) >= ((ma2 * 256) + 2):
                ma2 = 256 - a2
                print('Marcara da rede: \033[0;0;34m255.255.{:.0f}.0\033[m'.format(ma2))
                break
    if ma > 65534:
        a2 = 0
        print('A quantidade de máquinas está fora da quantidade suportada pela rede.')
    if ma < 65535:
        print('Bits usados:\033[0;0;34m{}\033[m'.format(bit))
        print('Bits usados para a rede externa:\033[0;0;34m', 32 - bit, '\033[m')
        print('ID da rede: \033[0;0;34m192.168.0.0\033[m')
        if ma < 255:
            lma = a - 2
            fip = a - 1
            print('Boradcast: \033[0;0;34m192.168.0.{}\033[m'.format(fip))
        if ma >= 255:
            lma = a2 * 256 - 2
            fip = a2 - 1
            print('Broadcast: \033[0;0;34m192.168.{}.255\033[m'.format(fip))

        print('IPv4 Classe C: \033[0;0;34m{}\033[m computadores'.format(lma))

if classe == 'B':
    print()
    for a in (qm):
        bit = bit + 1
        if a >= (ma + 2) and (ma < 255):
            ma2 = 256 - a
            print('Mascara da rede: \033[0;0;34m255.255.255.{}\033[m'.format(ma2))
            if ma == 0:
                bit = bit - 1
            break

    if ma >= 255 and ma <= 65534:
        bit = 8
        ma2 = ma / 256
        for a2 in (qm):
            bit = bit + 1
            if (a2 * 256) >= ((ma2 * 256) + 2):
                ma2 = 256 - a2
                print('Marcara da rede: \033[0;0;34m255.255.{:.0f}.0\033[m'.format(ma2))
                break
    if ma >= 65535 and ma <= 1048574:
        qm2 = (2, 4, 8, 16)
        bit = 16
        ma3 = ma / 65536
        for a3 in (qm2):
            bit = bit + 1
            if (a3 * 65536) >= (ma3 * 65536 + 2):
                ma3 = 256 - a3
                print('Mascara da rede: \033[0;0;34m255.{}.0.0\033[m'.format(ma3))
                break

    if ma > 1048574:
        a2 = 0
        print('A quantidade de máquinas está fora da quantidade suportada pela rede.')
    if ma < 1048574:
        print('Bits usados:\033[0;0;34m{}\033[m'.format(bit))
        print('Bits usados para a rede externa:\033[0;0;34m', 32 - bit, '\033[m')
        print('ID da rede: \033[0;0;34m172.16.0.0\033[m')
        if ma < 255:
            lma = a - 2
            fip = a - 1
            print('Boradcast: \033[0;0;34m172.16.0.{}\033[m'.format(fip))
        if ma >= 255 and ma <= 65534:
            lma = a2 * 256 - 2
            fip = a2 - 1
            print('Broadcast: \033[0;0;34m172.16.{}.255\033[m'.format(fip))
        if ma >= 65535:
            lma = a3 * 65536 - 2
            fip = a3 + 15
            print('Broadcast: \033[0;0;34m172.{}.255.255\033[m'.format(fip))

        print('IPv4 Classe B: \033[0;0;34m{}\033[m computadores'.format(lma))

if classe == 'A':
    print()
    for a in (qm):
        bit = bit + 1
        if a >= (ma + 2) and (ma < 255):
            ma2 = 256 - a
            print('Mascara da rede: \033[0;0;34m255.255.255.{}\033[m'.format(ma2))
            if ma == 0:
                bit = bit - 1
            break

    if ma >= 255 and ma <= 65534:
        bit = 8
        ma2 = ma / 256
        for a2 in (qm):
            bit = bit + 1
            if (a2 * 256) >= ((ma2 * 256) + 2):
                ma2 = 256 - a2
                print('Marcara da rede: \033[0;0;34m255.255.{:.0f}.0\033[m'.format(ma2))
                break
    if ma >= 1048574 and ma <= 16777214:
        qm2 = (2, 4, 8, 16, 32, 64, 128, 256)
        bit = 16
        ma3 = ma / 65536
        for a3 in (qm2):
            bit = bit + 1
            if (a3 * 65536) >= (ma3 * 65536 + 2):
                ma3 = 256 - a3
                print('Mascara da rede: \033[0;0;34m255.{}.0.0\033[m'.format(ma3))
                break

    if ma > 16777214:
        a2 = 0
        print('A quantidade de máquinas está fora da quantidade suportada pela rede.')
    if ma < 16777214:
        print('Bits usados: \033[0;0;34m{}\033[m'.format(bit))
        print('Bits usados para a rede externa:\033[0;0;34m', 32 - bit, '\033[m')
        print('ID da rede: \033[0;0;34m10.0.0.0\033[m')
        if ma < 255:
            lma = a - 2
            fip = a - 1
            print('Boradcast: \033[0;0;34m10.0.0.{}\033[m'.format(fip))
        if ma >= 255 and ma <= 65534:
            lma = a2 * 256 - 2
            fip = a2 - 1
            print('Broadcast:\033[0;0;34m 10.0.{}.255\033[m'.format(fip))
        if ma >= 65535:
            lma = a3 * 65536 - 2
            fip = a3 - 1
            print('Broadcast: \033[0;0;34m10.{}.255.255\033[m'.format(fip))

        print('IPv4 Classe A: \033[0;0;34m{}\033[m computadores'.format(lma))
