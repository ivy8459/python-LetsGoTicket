# python-LetsGoTicket
member={
    '曾志義', '林珈儀', '王小明', '黃小花','陳安安', '李建叡', '余冠柔'
    }
    
productlist = {
    '【飯店】':'漢來海港餐廳、大八大飯店\n',
    '【王品集團】':'王品台塑牛排、夏慕尼、陶板屋、西堤、小蒙牛、舒果、原燒、藝奇、品田牧場\n',
    '【其他連鎖餐廳】':'可利亞燒肉、東大門、千葉火鍋、全省素食\n',
    '【影城】':'威秀、喜滿客、環球、三多、奧斯卡、義大國賓、In89駁二電影院\n',
    '【展覽活動】':'大帑殿KTV、大英博物館木乃伊展、亞洲插畫年度大賞、每天來點負能量特展、卡娜赫拉的愜意小鎮特展\n',
    '【遊樂園】':'義大遊樂世界、花蓮遠雄海洋公園、屏東海生館、劍湖山、六福村、小人國、麗寶樂園'
    }


print('╠═╬═ ►Let’s Go樂吃購票券網◄ ═╬═╣')

print('∴∵∴∵∴加入會員享多重優惠∴∵∴∵∴')


func = input('瀏覽商品請輸入1\n加入會員請輸入2\n查看所有合作廠商請輸入3\n退換票券請輸入4\n')

if (int(func) == 1):    
    print('餐券\n電影票\n展覽活動\n遊樂園\n')
    category=input('請選擇商品類別\n')

    if(category=='餐券'):
        A={}
        restaurant=('漢來海港','大八大飯店','可利亞燒肉','千葉火鍋','東大門','全省素食',
        '王品台塑牛排','夏慕尼','陶板屋','西堤','小蒙牛','舒果','原燒','藝奇','品田牧場')
        A[restaurant] = '餐券'
        print(A)
        sortA = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortA == 'sort'):
            food = [
                (835,'漢來海港'),(770,'大八大飯店'),(530,'可利亞燒肉'),(370,'千葉火鍋'),(560,'東大門'),(580,'全省素食'),(1335,'王品台塑牛排'),
                (1040,'夏慕尼'),(580,'陶板屋'),(530,'西堤'),(635,'小蒙牛'),(425,'舒果'),(695,'原燒'),(730,'藝奇'),(360,'品田牧場')
                ]
            print(sorted(food, reverse = False))

        productA = input('請輸入您想查看的商品名稱\n')
        import math

        class 漢來海港:
            def intro(self):
                return"高雄市左營區博愛二路777號"
            def origin(self):
                return"原價 913元"
            def discount(self):
                return"特價 835元"
        class 大八大飯店:
            def intro(self):
                return"高雄市左營區裕誠路486號"
            def origin(self):
                return"原價 880元"
            def discount(self):
                return"特價 770元"        
        class 可利亞燒肉:
            def intro(self):
                return"高雄市左營區博愛四路1號"
            def origin(self):
                return"原價 582元"
            def discount(self):
                return"特價 530元"
        class 千葉火鍋:
            def intro(self):
                return"高雄市左營區自由三路100號"
            def origin(self):
                return"原價 395元"
            def discount(self):
                return"特價 370元"
        class 東大門:
            def intro(self):
                return"高雄市鳥松區公園路45號"
            def origin(self):
                return"原價 625元"
            def discount(self):
                return"特價 560元"
        class 全省素食:
            def intro(self):
                return"高雄市苓雅區四維二路359號"
            def origin(self):
                return"原價 726元"
            def discount(self):
                return"特價 580元"
        class 王品台塑牛排:
            def intro(self):
                return"高雄市新興區中正三路88號"
            def origin(self):
                return"原價 1485元"
            def discount(self):
                return"特價 1335元"
        class 夏慕尼:
            def intro(self):
                return"高雄市前金區五福三路29號"
            def origin(self):
                return"原價 1133元"
            def discount(self):
                return"特價 1040元"
        class 陶板屋:
            def intro(self):
                return"高雄市裕誠路475號"
            def origin(self):
                return"原價 625元"
            def discount(self):
                return"特價 580元"
        class 西堤:
            def intro(self):
                return"高雄市左營區富國路302號"
            def origin(self):
                return"原價 570元"
            def discount(self):
                return"特價 530元"
        class 小蒙牛:
            def intro(self):
                return"高雄市楠梓區藍田路288號"
            def origin(self):
                return"原價 680元"
            def discount(self):
                return"特價 635元"
        class 舒果:
            def intro(self):
                return"高雄市左營區博愛三路1號2樓"
            def origin(self):
                return"原價 438元"
            def discount(self):
                return"特價 425元"
        class 原燒:
            def intro(self):
                return"高雄市苓雅區中山二路410號"
            def origin(self):
                return"原價 741元"
            def discount(self):
                return"特價 695元"
        class 藝奇:
            def intro(self):
                return"高雄夢時代7F"
            def origin(self):
                return"原價 768元"
            def discount(self):
                return"特價 730元"
        class 品田牧場:
            def intro(self):
                return"高雄市前金區中山二路507號"
            def origin(self):
                return"原價 372元"
            def discount(self):
                return"特價 360元"
                   
        if (productA == '漢來海港'):
            hanlai = 漢來海港()
            print(hanlai.intro())
            print(hanlai.origin())
            print(hanlai.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(835*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(835*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價835元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(835*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價835元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(835*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(835*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(835*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')                

        elif (productA == '大八大飯店'):
            daba = 大八大飯店()
            print(daba.intro())
            print(daba.origin())
            print(daba.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(770*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(770*0.85*number),'元\n謝謝惠顧！')

                    if (login == False):
                        print ('非會員 特價770元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(770*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價770元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(770*number),'元\n謝謝惠顧！')
                
                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(770*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(770*0.85*number),'元\n謝謝惠顧！')

            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '可利亞燒肉'):
            korea = 可利亞燒肉()
            print(korea.intro())
            print(korea.origin())
            print(korea.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價530元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價530元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')                               
            
            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '千葉火鍋'):
            hotpot = 千葉火鍋()
            print(hotpot.intro())
            print(hotpot.origin())
            print(hotpot.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(370*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(370*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價370元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(370*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價370元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(370*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(370*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(370*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '東大門'):
            dong = 東大門()
            print(dong.intro())
            print(dong.origin())
            print(dong.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(560*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(560*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價560元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(560*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價560元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(560*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(560*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(560*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '全省素食'):
            veg = 全省素食()
            print(veg.intro())
            print(veg.origin())
            print(veg.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價580元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價580元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
           
        elif (productA == '王品台塑牛排'):
            wangsteak = 王品台塑牛排()
            print(wangsteak.intro())
            print(wangsteak.origin())
            print(wangsteak.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(1335*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1335*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價1335元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1335*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價1335元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1335*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(1335*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1335*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '夏慕尼'):
            chamonix = 夏慕尼()
            print(chamonix.intro())
            print(chamonix.origin())
            print(chamonix.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(1040*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1040*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價1040元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1040*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價1040元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1040*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(1040*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1040*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '陶板屋'):
            tokiya = 陶板屋()
            print(tokiya.intro())
            print(tokiya.origin())
            print(tokiya.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價580元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價580元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '西堤'):
            tasty = 西堤()
            print(tasty.intro())
            print(tasty.origin())
            print(tasty.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價530元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價530元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '小蒙牛'):
            cow = 小蒙牛()
            print(cow.intro())
            print(cow.origin())
            print(cow.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(635*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(635*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價635元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(635*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價635元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(635*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(635*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(635*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '舒果'):
            sufood = 舒果()
            print(sufood.intro())
            print(sufood.origin())
            print(sufood.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(425*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(425*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價425元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(425*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價425元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(425*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(425*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(425*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '原燒'):
            yuan = 原燒()
            print(yuan.intro())
            print(yuan.origin())
            print(yuan.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(695*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(695*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價695元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(695*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價695元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(695*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(695*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(695*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '藝奇'):
            ichi = 藝奇()
            print(ichi.intro())
            print(ichi.origin())
            print(ichi.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(730*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(730*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價730元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(730*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價730元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(730*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(730*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(730*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '品田牧場'):
            farm = 品田牧場()
            print(farm.intro())
            print(farm.origin())
            print(farm.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(360*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(360*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價360元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(360*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價360元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(360*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(360*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(360*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
            
        else:
            print('Error! 請重新輸入')

    elif(category=='電影票'):
        B={}
        cinema=('威秀影城','喜滿客','環球影城','三多影城','奧斯卡影城','義大國賓影城','In89駁二電影院')
        B[cinema] = '電影票'
        print(B)
        sortB = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortB == 'sort'):
            theater = [
                (220,'威秀影城'),(205,'喜滿客'),(195,'環球影城'),(165,'三多影城'),(180,'奧斯卡影城'),(170,'義大國賓影城'),(215,'In89駁二電影院')
                ]
            print(sorted(theater, reverse = False))

        productB = input('請輸入您想查看的商品名稱\n')
        import math

        class 威秀影城:
            def intro(self):
                return"高雄大遠百"
            def origin(self):
                return"原價 270元"
            def discount(self):
                return"特價 220元"
        class 喜滿客:
            def intro(self):
                return"高雄夢時代"
            def origin(self):
                return"原價 260元"
            def discount(self):
                return"特價 205元"
        class 環球影城:
            def intro(self):
                return"高雄市苓雅區大順三路108號"
            def origin(self):
                return"原價 240元"
            def discount(self):
                return"特價 195元"
        class 三多影城:
            def intro(self):
                return"高雄市苓雅區三多四路123號"
            def origin(self):
                return"原價 215元"
            def discount(self):
                return"特價 165元"
        class 奧斯卡影城:
            def intro(self):
                return"高雄市新興區仁智街287號"
            def origin(self):
                return"原價 250元"
            def discount(self):
                return"特價 180元"
        class 義大國賓影城:
            def intro(self):
                return"高雄義大世界"
            def origin(self):
                return"原價 240元"
            def discount(self):
                return"特價 170元"
        class In89駁二電影院:
            def intro(self):
                return"高雄駁二藝術特區"
            def origin(self):
                return"原價 270元"
            def discount(self):
                return"特價 215元"

        if (productB == '威秀影城'):
            vieshow = 威秀影城()
            print(vieshow.intro())
            print(vieshow.origin())
            print(vieshow.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(220*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(220*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價220元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(220*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價220元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(220*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(220*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(220*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '喜滿客'):
            cinemark = 喜滿客()
            print(cinemark.intro())
            print(cinemark.origin())
            print(cinemark.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(205*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(205*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價205元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(205*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價205元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(205*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(205*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(205*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '環球影城'):
            umovie = 環球影城()
            print(umovie.intro())
            print(umovie.origin())
            print(umovie.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(195*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(195*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價195元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(195*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價195元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(195*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(195*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(195*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == '三多影城'):
            sando = 三多影城()
            print(sando.intro())
            print(sando.origin())
            print(sando.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(165*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(165*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價165元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(165*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價165元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(165*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(165*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(165*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == '奧斯卡影城'):
            oscar = 奧斯卡影城()
            print(oscar.intro())
            print(oscar.origin())
            print(oscar.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(108*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價180元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價180元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(180*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '義大國賓影城'):
            eda = 義大國賓影城()
            print(eda.intro())
            print(eda.origin())
            print(eda.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(170*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(170*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價170元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(170*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價170元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(170*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(170*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(170*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == 'In89駁二電影院'):
            in89 = In89駁二電影院()
            print(in89.intro())
            print(in89.origin())
            print(in89.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(215*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(215*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價215元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(215*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價215元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(215*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(215*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(215*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        else:
            print('Error! 請重新輸入')

    elif(category=='展覽活動'):
        C={}
        activity=('大帑殿KTV','大英博物館木乃伊展','亞洲插畫年度大賞','每天來點負能量特展','卡娜赫拉的愜意小鎮特展')
        C[activity] = '展覽活動'
        print(C)
        sortC = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortC == 'sort'):
            entertain = [
                (430,'大帑殿KTV'),(280,'大英博物館木乃伊展'),(120,'亞洲插畫年度大賞'),(100,'每天來點負能量特展'),(180,'卡娜赫拉的愜意小鎮特展')
                ]
            print(sorted(entertain, reverse = False))
        productC = input('請輸入您想查看的商品名稱\n')
        import math

        class 大帑殿KTV:
            def intro(self):
                return"高雄地區首屈一指庭園式KTV，全面使用無線麥克風以及大型液晶螢幕，點歌系統也升級為觸控式的冷光操作介面，提供北高雄消費者一個安全舒適的歡唱空間！\n營業時間：24H\n預約電話：07-552-9989\n地址：高雄市明華路633號"
            def origin(self):
                return"原價 500元"
            def discount(self):
                return"特價 430元"
        
        class 大英博物館木乃伊展:
            def intro(self):
                return"「大英博物館藏埃及木乃伊：探索古代生活」特展，將完整呈現遠古時期的6具木乃伊、棺槨、陪葬品及石碑等超過200件物品，藉此透視古埃及尚未公諸於世的秘密以及探索當時埃及人的生活。\n展期：2017/11/14(二) ~ 2018/02/18(日)\n地點：故宮博物院"
            def origin(self):
                return"原價 350元"
            def discount(self):
                return"特價 280元"

        class 亞洲插畫年度大賞:
            def intro(self):
                return"為期三個月的國際插畫大展，集結了250位來自台灣、日本等17國的優秀創作者，而且展示的插畫作品高達1250幅！\n展期：2017/12/16(六) ~ 2018/03/04(日)\n地點：松山文創園區"
            def origin(self):
                return"原價 180元"
            def discount(self):
                return"特價 120元"

        class 每天來點負能量特展:
            def intro(self):
                return"70萬粉絲每天中箭無數，給你每天負負得正的力量。網路超人氣粉絲團《每天來點負能量》，今年聖誕節嘲諷開展！\n展期：2017/12/22(五) ~ 2018/02/25(日)\n地點：松山文創園區"
            def origin(self):
                return"原價 280元"
            def discount(self):
                return"特價 100元"
        
        class 卡娜赫拉的愜意小鎮特展:
            def intro(self):
                return"蟬聯日本超人氣貼圖王的「卡娜赫拉」（Kanahei）首座大型個展，邀請大家與兔兔和P助一同來趟最療癒的魔法旅程！\n展期：2017/12/30(六) ~ 2018/03/25(日)\n地點：華珊創意園區"
            def origin(self):
                return"原價 280元"
            def discount(self):
                return"特價 180元"
        
        if (productC == '大帑殿KTV'):
            tempoktv = 大帑殿KTV()
            print(tempoktv.intro())
            print(tempoktv.origin())
            print(tempoktv.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價430元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價430元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productC == '大英博物館木乃伊展'):
            mummy = 大英博物館木乃伊展()
            print(mummy.intro())
            print(mummy.origin())
            print(mummy.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(280*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(280*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價280元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(280*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價280元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(280*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(280*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(280*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productC == '亞洲插畫年度大賞'):
            draw = 亞洲插畫年度大賞()
            print(draw.intro())
            print(draw.origin())
            print(draw.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(120*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(120*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價120元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(120*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價120元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(120*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(120*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(120*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productC == '每天來點負能量特展'):
            energy = 每天來點負能量特展()
            print(energy.intro())
            print(energy.origin())
            print(energy.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(100*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(100*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價100元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(100*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價100元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(100*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(100*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(100*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productC == '卡娜赫拉的愜意小鎮特展'):
            kanahei = 卡娜赫拉的愜意小鎮特展()
            print(kanahei.intro())
            print(kanahei.origin())
            print(kanahei.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(180*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價180元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價180元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(180*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        else:
            print('Error! 請重新輸入')

    elif(category=='遊樂園'):
        D={}
        park=('義大遊樂世界','花蓮遠雄海洋公園','屏東海生館','劍湖山','六福村','小人國','麗寶樂園')
        D[park] = '遊樂園'
        print(D)
        sortD = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortD == 'sort'):
            fun = [
                (700,'義大遊樂世界'),(800,'花蓮遠雄海洋公園'),(430,'屏東海生館'),(490,'劍湖山'),(520,'六福村'),(450,'小人國'),(490,'麗寶樂園')
                ]
            print(sorted(fun, reverse = False))
        productD = input('請輸入您想查看的商品名稱\n')
        import math

        class 義大遊樂世界:
            def intro(self):
                return"高雄市大樹區學城路一段10號"
            def origin(self):
                return"原價 899元"
            def discount(self):
                return"特價 700元"
        class 花蓮遠雄海洋公園:
            def intro(self):
                return"花蓮縣壽豐鄉鹽寮村福德189號"
            def origin(self):
                return"原價 890元"
            def discount(self):
                return"特價 800元"
        class 屏東海生館:
            def intro(self):
                return"屏東縣車城鄉後灣路2號"
            def origin(self):
                return"原價 450元"
            def discount(self):
                return"特價 430元"
        class 劍湖山:
            def intro(self):
                return"雲林縣古坑鄉永光村大湖口67號"
            def origin(self):
                return"原價 799元"
            def discount(self):
                return"特價 490元"
        class 六福村:
            def intro(self):
                return"新竹縣關西鎮仁安里拱子溝60號"
            def origin(self):
                return"原價 999元"
            def discount(self):
                return"特價 520元"
        class 小人國:
            def intro(self):
                return"桃園市龍潭區高原路891號"
            def origin(self):
                return"原價 799元"
            def discount(self):
                return"特價 450元"
        class 麗寶樂園:
            def intro(self):
                return"台中市后里區福容路8號"
            def origin(self):
                return"原價 800元"
            def discount(self):
                return"特價 490元"
        
        if (productD == '義大遊樂世界'):
            edaworld = 義大遊樂世界()
            print(edaworld.intro())
            print(edaworld.origin())
            print(edaworld.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(700*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(700*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價700元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(700*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價700元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(700*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(700*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(700*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '花蓮遠雄海洋公園'):
            hualien = 花蓮遠雄海洋公園()
            print(hualien.intro())
            print(hualien.origin())
            print(hualien.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(800*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(800*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價800元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(800*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價800元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(800*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(800*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(800*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '屏東海生館'):
            pintung = 屏東海生館()
            print(pintung.intro())
            print(pintung.origin())
            print(pintung.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價430元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價430元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '劍湖山'):
            janfusan = 劍湖山()
            print(janfusan.intro())
            print(janfusan.origin())
            print(janfusan.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價490元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價490元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '六福村'):
            village = 六福村()
            print(village.intro())
            print(village.origin())
            print(village.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(520*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(520*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價520元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(520*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價520元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(520*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(520*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(520*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '小人國'):
            mini = 小人國()
            print(mini.intro())
            print(mini.origin())
            print(mini.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(450*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(450*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價450元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(450*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價450元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(450*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(450*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(450*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '麗寶樂園'):
            lihpao = 麗寶樂園()
            print(lihpao.intro())
            print(lihpao.origin())
            print(lihpao.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                membership = input('請問您是會員嗎，請輸入Yes/No\n立即加入會員請輸入Join\n')                            
                if (membership == 'Yes'):
                    name=input('請輸入您的名字\n')
                    login = name in member
                    if (login == True):
                        print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')
                    
                    if (login == False):
                        print ('非會員 特價490元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*number),'元\n謝謝惠顧！')

                elif (membership == 'No'):
                    print('非會員 特價490元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*number),'元\n謝謝惠顧！')

                elif (membership == 'Join'):
                    username=input('歡迎您加入會員，請輸入您的姓名\n')
                    member.add(username)
                    print('恭喜您成功加入會員!!\n')
                    print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')                               

            elif (int(buy) == 2):
                print('您已取消訂購')
        
        else:
            print('Error! 請重新輸入')

    else:
        print('請重新輸入')


elif (int(func) == 2):
    username=input('請輸入您的姓名\n')
    member.add(username)
    print('恭喜您成功加入會員!!\n') 
    print('餐券\n電影票\n展覽活動\n遊樂園\n')
    category=input('請選擇商品類別\n')

    if(category=='餐券'):
        A={}
        restaurant=('漢來海港','大八大飯店','可利亞燒肉','千葉火鍋','東大門','全省素食',
        '王品台塑牛排','夏慕尼','陶板屋','西堤','小蒙牛','舒果','原燒','藝奇','品田牧場')
        A[restaurant] = '餐券'
        print(A)
        sortA = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortA == 'sort'):
            food = [
                (835,'漢來海港'),(770,'大八大飯店'),(530,'可利亞燒肉'),(370,'千葉火鍋'),(560,'東大門'),(580,'全省素食'),(1335,'王品台塑牛排'),
                (1040,'夏慕尼'),(580,'陶板屋'),(530,'西堤'),(635,'小蒙牛'),(425,'舒果'),(695,'原燒'),(730,'藝奇'),(360,'品田牧場')
                ]
            print(sorted(food, reverse = False))

        productA = input('請輸入您想查看的商品名稱\n')
        import math

        class 漢來海港:
            def intro(self):
                return"高雄市左營區博愛二路777號"
            def origin(self):
                return"原價 913元"
            def discount(self):
                return"特價 835元"
        class 大八大飯店:
            def intro(self):
                return"高雄市左營區裕誠路486號"
            def origin(self):
                return"原價 880元"
            def discount(self):
                return"特價 770元"        
        class 可利亞燒肉:
            def intro(self):
                return"高雄市左營區博愛四路1號"
            def origin(self):
                return"原價 582元"
            def discount(self):
                return"特價 530元"
        class 千葉火鍋:
            def intro(self):
                return"高雄市左營區自由三路100號"
            def origin(self):
                return"原價 395元"
            def discount(self):
                return"特價 370元"
        class 東大門:
            def intro(self):
                return"高雄市鳥松區公園路45號"
            def origin(self):
                return"原價 625元"
            def discount(self):
                return"特價 560元"
        class 全省素食:
            def intro(self):
                return"高雄市苓雅區四維二路359號"
            def origin(self):
                return"原價 726元"
            def discount(self):
                return"特價 580元"
        class 王品台塑牛排:
            def intro(self):
                return"高雄市新興區中正三路88號"
            def origin(self):
                return"原價 1485元"
            def discount(self):
                return"特價 1335元"
        class 夏慕尼:
            def intro(self):
                return"高雄市前金區五福三路29號"
            def origin(self):
                return"原價 1133元"
            def discount(self):
                return"特價 1040元"
        class 陶板屋:
            def intro(self):
                return"高雄市裕誠路475號"
            def origin(self):
                return"原價 625元"
            def discount(self):
                return"特價 580元"
        class 西堤:
            def intro(self):
                return"高雄市左營區富國路302號"
            def origin(self):
                return"原價 570元"
            def discount(self):
                return"特價 530元"
        class 小蒙牛:
            def intro(self):
                return"高雄市楠梓區藍田路288號"
            def origin(self):
                return"原價 680元"
            def discount(self):
                return"特價 635元"
        class 舒果:
            def intro(self):
                return"高雄市左營區博愛三路1號2樓"
            def origin(self):
                return"原價 438元"
            def discount(self):
                return"特價 425元"
        class 原燒:
            def intro(self):
                return"高雄市苓雅區中山二路410號"
            def origin(self):
                return"原價 741元"
            def discount(self):
                return"特價 695元"
        class 藝奇:
            def intro(self):
                return"高雄夢時代7F"
            def origin(self):
                return"原價 768元"
            def discount(self):
                return"特價 730元"
        class 品田牧場:
            def intro(self):
                return"高雄市前金區中山二路507號"
            def origin(self):
                return"原價 372元"
            def discount(self):
                return"特價 360元"
                   
        if (productA == '漢來海港'):
            hanlai = 漢來海港()
            print(hanlai.intro())
            print(hanlai.origin())
            print(hanlai.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(835*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(835*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')          
                                 

        elif (productA == '大八大飯店'):
            daba = 大八大飯店()
            print(daba.intro())
            print(daba.origin())
            print(daba.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(770*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(770*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '可利亞燒肉'):
            korea = 可利亞燒肉()
            print(korea.intro())
            print(korea.origin())
            print(korea.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '千葉火鍋'):
            hotpot = 千葉火鍋()
            print(hotpot.intro())
            print(hotpot.origin())
            print(hotpot.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(370*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(370*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '東大門'):
            dong = 東大門()
            print(dong.intro())
            print(dong.origin())
            print(dong.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(560*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(560*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
                    
        elif (productA == '全省素食'):
            veg = 全省素食()
            print(veg.intro())
            print(veg.origin())
            print(veg.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
           
        elif (productA == '王品台塑牛排'):
            wangsteak = 王品台塑牛排()
            print(wangsteak.intro())
            print(wangsteak.origin())
            print(wangsteak.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(1335*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1335*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '夏慕尼'):
            chamonix = 夏慕尼()
            print(chamonix.intro())
            print(chamonix.origin())
            print(chamonix.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(1040*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(1040*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '陶板屋'):
            tokiya = 陶板屋()
            print(tokiya.intro())
            print(tokiya.origin())
            print(tokiya.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(580*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(580*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '西堤'):
            tasty = 西堤()
            print(tasty.intro())
            print(tasty.origin())
            print(tasty.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(530*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(530*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        elif (productA == '小蒙牛'):
            cow = 小蒙牛()
            print(cow.intro())
            print(cow.origin())
            print(cow.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(635*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(635*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '舒果'):
            sufood = 舒果()
            print(sufood.intro())
            print(sufood.origin())
            print(sufood.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(425*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(425*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '原燒'):
            yuan = 原燒()
            print(yuan.intro())
            print(yuan.origin())
            print(yuan.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(695*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(695*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '藝奇'):
            ichi = 藝奇()
            print(ichi.intro())
            print(ichi.origin())
            print(ichi.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(730*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(730*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productA == '品田牧場'):
            farm = 品田牧場()
            print(farm.intro())
            print(farm.origin())
            print(farm.discount())
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(360*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(360*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
            
        else:
            print('Error! 請重新輸入')

    elif(category=='電影票'):
        B={}
        cinema=('威秀影城','喜滿客','環球影城','三多影城','奧斯卡影城','義大國賓影城','In89駁二電影院')
        B[cinema] = '電影票'
        print(B)
        sortB = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortB == 'sort'):
            theater = [
                (220,'威秀影城'),(205,'喜滿客'),(195,'環球影城'),(165,'三多影城'),(180,'奧斯卡影城'),(170,'義大國賓影城'),(215,'In89駁二電影院')
                ]
            print(sorted(theater, reverse = False))

        productB = input('請輸入您想查看的商品名稱\n')
        import math

        class 威秀影城:
            def intro(self):
                return"高雄大遠百"
            def origin(self):
                return"原價 270元"
            def discount(self):
                return"特價 220元"
        class 喜滿客:
            def intro(self):
                return"高雄夢時代"
            def origin(self):
                return"原價 260元"
            def discount(self):
                return"特價 205元"
        class 環球影城:
            def intro(self):
                return"高雄市苓雅區大順三路108號"
            def origin(self):
                return"原價 240元"
            def discount(self):
                return"特價 195元"
        class 三多影城:
            def intro(self):
                return"高雄市苓雅區三多四路123號"
            def origin(self):
                return"原價 215元"
            def discount(self):
                return"特價 165元"
        class 奧斯卡影城:
            def intro(self):
                return"高雄市新興區仁智街287號"
            def origin(self):
                return"原價 250元"
            def discount(self):
                return"特價 180元"
        class 義大國賓影城:
            def intro(self):
                return"高雄義大世界"
            def origin(self):
                return"原價 240元"
            def discount(self):
                return"特價 170元"
        class In89駁二電影院:
            def intro(self):
                return"高雄駁二藝術特區"
            def origin(self):
                return"原價 270元"
            def discount(self):
                return"特價 215元"

        if (productB == '威秀影城'):
            vieshow = 威秀影城()
            print(vieshow.intro())
            print(vieshow.origin())
            print(vieshow.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(220*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(220*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '喜滿客'):
            cinemark = 喜滿客()
            print(cinemark.intro())
            print(cinemark.origin())
            print(cinemark.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(205*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(205*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '環球影城'):
            umovie = 環球影城()
            print(umovie.intro())
            print(umovie.origin())
            print(umovie.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(195*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(195*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == '三多影城'):
            sando = 三多影城()
            print(sando.intro())
            print(sando.origin())
            print(sando.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(165*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(165*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == '奧斯卡影城'):
            oscar = 奧斯卡影城()
            print(oscar.intro())
            print(oscar.origin())
            print(oscar.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(180*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productB == '義大國賓影城'):
            eda = 義大國賓影城()
            print(eda.intro())
            print(eda.origin())
            print(eda.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(170*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(170*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productB == 'In89駁二電影院'):
            in89 = In89駁二電影院()
            print(in89.intro())
            print(in89.origin())
            print(in89.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(215*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(215*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        else:
            print('Error! 請重新輸入')

    elif(category=='展覽活動'):
        C={}
        activity=('大帑殿KTV','大英博物館木乃伊展','亞洲插畫年度大賞','每天來點負能量特展','卡娜赫拉的愜意小鎮特展')
        C[activity] = '展覽活動'
        print(C)
        sortC = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortC == 'sort'):
            entertain = [
                (430,'大帑殿KTV'),(280,'大英博物館木乃伊展'),(120,'亞洲插畫年度大賞'),(100,'每天來點負能量特展'),(180,'卡娜赫拉的愜意小鎮特展')
                ]
            print(sorted(entertain, reverse = False))
        productC = input('請輸入您想查看的商品名稱\n')
        import math

        class 大帑殿KTV:
            def intro(self):
                return"高雄地區首屈一指庭園式KTV，全面使用無線麥克風以及大型液晶螢幕，點歌系統也升級為觸控式的冷光操作介面，提供北高雄消費者一個安全舒適的歡唱空間！\n營業時間：24H\n預約電話：07-552-9989\n地址：高雄市明華路633號"
            def origin(self):
                return"原價 500元"
            def discount(self):
                return"特價 430元"
        
        class 大英博物館木乃伊展:
            def intro(self):
                return"「大英博物館藏埃及木乃伊：探索古代生活」特展，將完整呈現遠古時期的6具木乃伊、棺槨、陪葬品及石碑等超過200件物品，藉此透視古埃及尚未公諸於世的秘密以及探索當時埃及人的生活。\n展期：2017/11/14(二) ~ 2018/02/18(日)\n地點：故宮博物院"
            def origin(self):
                return"原價 350元"
            def discount(self):
                return"特價 280元"

        class 亞洲插畫年度大賞:
            def intro(self):
                return"為期三個月的國際插畫大展，集結了250位來自台灣、日本等17國的優秀創作者，而且展示的插畫作品高達1250幅！\n展期：2017/12/16(六) ~ 2018/03/04(日)\n地點：松山文創園區"
            def origin(self):
                return"原價 180元"
            def discount(self):
                return"特價 120元"

        class 每天來點負能量特展:
            def intro(self):
                return"70萬粉絲每天中箭無數，給你每天負負得正的力量。網路超人氣粉絲團《每天來點負能量》，今年聖誕節嘲諷開展！\n展期：2017/12/22(五) ~ 2018/02/25(日)\n地點：松山文創園區"
            def origin(self):
                return"原價 280元"
            def discount(self):
                return"特價 100元"
        
        class 卡娜赫拉的愜意小鎮特展:
            def intro(self):
                return"蟬聯日本超人氣貼圖王的「卡娜赫拉」（Kanahei）首座大型個展，邀請大家與兔兔和P助一同來趟最療癒的魔法旅程！\n展期：2017/12/30(六) ~ 2018/03/25(日)\n地點：華珊創意園區"
            def origin(self):
                return"原價 280元"
            def discount(self):
                return"特價 180元"
        
        if (productC == '大帑殿KTV'):
            tempoktv = 大帑殿KTV()
            print(tempoktv.intro())
            print(tempoktv.origin())
            print(tempoktv.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productC == '大英博物館木乃伊展'):
            mummy = 大英博物館木乃伊展()
            print(mummy.intro())
            print(mummy.origin())
            print(mummy.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(280*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(280*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productC == '亞洲插畫年度大賞'):
            draw = 亞洲插畫年度大賞()
            print(draw.intro())
            print(draw.origin())
            print(draw.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(120*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(120*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productC == '每天來點負能量特展'):
            energy = 每天來點負能量特展()
            print(energy.intro())
            print(energy.origin())
            print(energy.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(100*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(100*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productC == '卡娜赫拉的愜意小鎮特展'):
            kanahei = 卡娜赫拉的愜意小鎮特展()
            print(kanahei.intro())
            print(kanahei.origin())
            print(kanahei.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(180*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(180*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        else:
            print('Error! 請重新輸入')

    elif(category=='遊樂園'):
        D={}
        park=('義大遊樂世界','花蓮遠雄海洋公園','屏東海生館','劍湖山','六福村','小人國','麗寶樂園')
        D[park] = '遊樂園'
        print(D)
        sortD = input('欲查看價位由低至高排序請輸入sort或按任意鍵繼續\n')
        if (sortD == 'sort'):
            fun = [
                (700,'義大遊樂世界'),(800,'花蓮遠雄海洋公園'),(430,'屏東海生館'),(490,'劍湖山'),(520,'六福村'),(450,'小人國'),(490,'麗寶樂園')
                ]
            print(sorted(fun, reverse = False))
        productD = input('請輸入您想查看的商品名稱\n')
        import math

        class 義大遊樂世界:
            def intro(self):
                return"高雄市大樹區學城路一段10號"
            def origin(self):
                return"原價 899元"
            def discount(self):
                return"特價 700元"
        class 花蓮遠雄海洋公園:
            def intro(self):
                return"花蓮縣壽豐鄉鹽寮村福德189號"
            def origin(self):
                return"原價 890元"
            def discount(self):
                return"特價 800元"
        class 屏東海生館:
            def intro(self):
                return"屏東縣車城鄉後灣路2號"
            def origin(self):
                return"原價 450元"
            def discount(self):
                return"特價 430元"
        class 劍湖山:
            def intro(self):
                return"雲林縣古坑鄉永光村大湖口67號"
            def origin(self):
                return"原價 799元"
            def discount(self):
                return"特價 490元"
        class 六福村:
            def intro(self):
                return"新竹縣關西鎮仁安里拱子溝60號"
            def origin(self):
                return"原價 999元"
            def discount(self):
                return"特價 520元"
        class 小人國:
            def intro(self):
                return"桃園市龍潭區高原路891號"
            def origin(self):
                return"原價 799元"
            def discount(self):
                return"特價 450元"
        class 麗寶樂園:
            def intro(self):
                return"台中市后里區福容路8號"
            def origin(self):
                return"原價 800元"
            def discount(self):
                return"特價 490元"
        
        if (productD == '義大遊樂世界'):
            edaworld = 義大遊樂世界()
            print(edaworld.intro())
            print(edaworld.origin())
            print(edaworld.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(700*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(700*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '花蓮遠雄海洋公園'):
            hualien = 花蓮遠雄海洋公園()
            print(hualien.intro())
            print(hualien.origin())
            print(hualien.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(800*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(800*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '屏東海生館'):
            pintung = 屏東海生館()
            print(pintung.intro())
            print(pintung.origin())
            print(pintung.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(430*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(430*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')

        elif (productD == '劍湖山'):
            janfusan = 劍湖山()
            print(janfusan.intro())
            print(janfusan.origin())
            print(janfusan.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '六福村'):
            village = 六福村()
            print(village.intro())
            print(village.origin())
            print(village.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(520*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(520*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '小人國'):
            mini = 小人國()
            print(mini.intro())
            print(mini.origin())
            print(mini.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(450*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(450*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        elif (productD == '麗寶樂園'):
            lihpao = 麗寶樂園()
            print(lihpao.intro())
            print(lihpao.origin())
            print(lihpao.discount())
            
            buy = input('1:結帳\n2:取消訂購\n')
            if (int(buy) == 1):
                new = input('新會員您好，請再次輸入您的姓名以取得驗證\n')
                check = new in member                            
                if (check == True):
                    print('►會員獨享85折◄',math.ceil(490*0.85),'元')
                    number=int(input('請輸入欲購買張數\n'))
                    print('總金額',math.ceil(490*0.85*number),'元\n謝謝惠顧！')
                if (check == False):
                    print('驗證失敗，請重新加入會員')
            elif (int(buy) == 2):
                print('您已取消訂購')
        
        else:
            print('Error! 請重新輸入')

    else:
        print('請重新輸入')
    
elif (int(func) == 3):    
    for allproduct in productlist:
        print(allproduct)
        print(productlist[allproduct])

      

else:
    print('請輸入有效功能代號')
