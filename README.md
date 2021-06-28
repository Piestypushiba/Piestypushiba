const Discord = require('discord.js');
const client = new Discord.Client();

const balcerowicz = [
    "https://imgur.com/uTfkN3S",
    "https://imgur.com/nHZdnU7",
    "https://imgur.com/Dhj1T4W",
    "https://imgur.com/tv31q5S",
    "https://imgur.com/6DQNxOW",
    "https://imgur.com/RJCdR8q",
    "https://imgur.com/kUjYNYP",
    "https://imgur.com/N8k3Oqb",
    "https://imgur.com/ZgvYuDM",
    "https://imgur.com/0wANcI0",
    "https://imgur.com/ECHtbLH",
    "https://imgur.com/qP8mbDu",
    "https://imgur.com/8YLacYp",
    "https://imgur.com/YDghxdt",
    "https://imgur.com/DzxOHLX",
    "https://imgur.com/nfYZ1Fj",
    "https://imgur.com/DyH8K9u",
    "https://imgur.com/jkZAR7S",
    "https://imgur.com/MC1OvyT",
    "https://imgur.com/RD5Jkge",
    "https://imgur.com/0WIVNTo",
    "https://imgur.com/QOOBAaL",
    "https://imgur.com/UcMVlEp",
    "https://imgur.com/r8l2ku9",
    "https://imgur.com/5IDCKrz",
    "https://imgur.com/IXz56kb",
    "https://imgur.com/fMz0D4H",
    "https://imgur.com/5vdyXQ0",
    "https://imgur.com/Bdb76H9",
    "https://imgur.com/AjMrfjf",
    "https://imgur.com/5Gkrplf",
    "https://imgur.com/CuO6EK2",
    "https://imgur.com/2B4fEMl",
    "https://imgur.com/edYBoGb",
    "https://imgur.com/s7ExBVY",
    "https://imgur.com/zL81bNP",
    "https://imgur.com/ukMT86p",
    "https://imgur.com/m0HEjch",
    "https://imgur.com/hXAkGi3",
    "https://imgur.com/Og9M1ot",
    "https://imgur.com/9wVlOM9",
    "https://imgur.com/GWqmSPn",
    "https://imgur.com/3BdNCfe",
    "https://imgur.com/vWSJ0Yr",
    "https://imgur.com/q89fssF",
    "https://imgur.com/NIy6Ut4",
    "https://imgur.com/Z7jhALd",
    "https://imgur.com/hwwS6v5",
    "https://imgur.com/YA6RI39",
    "https://imgur.com/IjOGGTg",
    "https://imgur.com/VO74VSm",
    "https://imgur.com/LUFhIeO",
    "https://imgur.com/avAQC6E",
    "https://imgur.com/oVVyZfM",
    "https://imgur.com/HWmEm1x",
    "https://imgur.com/I2Ozoly",
    "https://imgur.com/MG8YD9d",
    "https://imgur.com/kInGtVz",
    "https://imgur.com/0YNQCrF",
    "https://imgur.com/5TH9qd6",
    "https://imgur.com/CV8bHBC",
    "https://imgur.com/7q536yw",
    "https://imgur.com/WR2Ih53",
    "https://imgur.com/4Ggp6yD",
    "https://imgur.com/efUGN2f",
    "https://imgur.com/fDNXgTG",
    "https://imgur.com/TXZfzOB",
    "https://imgur.com/TnPUaXK",
    "https://imgur.com/LvSx5Gh",
    "https://imgur.com/GMrIgOU",
    "https://imgur.com/NwSqx6Q",
    "https://imgur.com/eVQzL8o",
    "https://imgur.com/3F4NaIB",
    "https://imgur.com/shnraU6",
    "https://imgur.com/kAHCLZt",
    "https://imgur.com/yUlOwDe",
    "https://imgur.com/rHXVgyL",
    "https://imgur.com/0LSqNEg",
    "https://imgur.com/HeaP7lt",
    "https://imgur.com/dn68oC9",
    "https://imgur.com/70qKMao",
    "https://imgur.com/DpBWNM4",
    "https://imgur.com/AbeWU83",
    "https://imgur.com/W8tfMOW",
    "https://imgur.com/BF0hk2o",
    "https://imgur.com/OuKkBU1",
    "https://imgur.com/EQeThNb",
    "https://imgur.com/cjLEBZW",
    "https://imgur.com/Sdg0jMf",
    "https://imgur.com/IakZ3jI",
    "https://imgur.com/LwqSDfb",
    "https://imgur.com/syvyIpl",
    "https://imgur.com/qbs80qE",
    "https://imgur.com/YXEFFnL",
    "https://imgur.com/M8XaRbu" //5 czerwca ostatnie
];

const seksZPedalami = [
	"Czy państwo potrzebuje biurokracji aby prawidłowo działać?",
    "Jak dużą władzę rodzice powinni mieć nad swoimi dziećmi?", 
    "Czy wolna wola istnieje? Jak ją zdefiniować?",
    "Do czego powinna dążyć ludzkość?",
    "Gdyby dziecko jakimś cudem przetrwało i dorosło w dziczy, jak bardzo „ludzkie” by było bez wpływu społeczeństwa i kultury?",
    "Co by się stało, gdyby średnia długość życia człowieka wydłużyła się do 500 lat?",
    "Czy religia kiedykolwiek zniknie?",
    "Czy cierpienie wzmacnia człowieka?",
    "Jakie korzyści społeczeństwo czerpie ze sztuki? Czy są jakieś jej wady?",
    "Czy jeśli określimy, że wolność jest możliwością robienia tego, co chcemy, to zwierzęta są wolniejsze niż ludzie?",
    "Czy ludzkość zmierza w dobrym, czy w złym kierunku?",
    "Czy filozofia kiedykolwiek prowadzi do odpowiedzi, czy jedynie do większej ilości pytań? Czy ma sens?",
    "Jak zdefiniowałbyś polskość?",
    "Czy patriotyzm jest potrzebny?",
    "Czy imigranci powinni zostać poddani skrupulatnej selekcji?",
    "Czy alkohol, papierosy, narkotyki i inne używki powinny być legalne?",
    "Czy człowiek jest w stanie powstrzymać katastrofę klimatyczną?",
    "Czy cel uświęca środki?",
    "Skąd wiesz, że podejmujesz świadome decyzje?",
    "Czy toksyczna męskość jest problemem XXI wieku?",
    "Czy w dzisiejszych czasach feminizm jest potrzebny?",
    "Bardziej przydatna jest wiedza czy inteligencja? Którą byś wybrał?",
    "Najbardziej znanym cytatem Kartezjusza jest “Myślę, więc jestem”. Czy zgadzasz się z tą konkluzją?",
    "Byt kreuje świadomość czy świadomość kreuje byt?",
    "Co bardziej kształtuje dzieje ludzkości - bezimienne masy, czy wybitne indywidua?",
    "Lepiej posiadać szeroką wiedzę na jeden temat, czy ogólną na wiele tematów?",
    "Czy w XXI wieku społeczeństwo jest podzielone na klasy?",
    "Czy katolicyzm jest nierozerwalną częścią tożsamości polskiej?",
    "Czy Polska powinna odzyskać utracone w swojej przeszłości tereny?",
    "Gdzie dokładnie zaczyna się i kończy wolność drugiego człowieka?",
    "Czy uważasz, że ludzie dzielą się na lepszych i gorszych?",
    "Ważniejsza jest dla ciebie wolność czy bezpieczeństwo?",
    "Czy ludobójstwo można usprawiedliwić jeśli zapewni w ostateczności wolność większej ilości osób?",
    "Czy da się zmienić ludzką naturę?",
    "Czy władza zawsze deprawuje?",
    "Czy litość jest słabością?",
    "Co zapewnia jednostce prawo do własności?",
    "Matematyka została odkryta czy wynaleziona? Czy spoglądanie na rzeczywistość z matematycznego punktu widzenia daje precyzyjną wizję świata?",
    "Czy istnieje coś takiego jak cywilizacja europejska? Jeśli tak, to czym ona dokładnie jest?",
    "Czy utrzymanie porządku społecznego jest ważniejsze od wolności ludzkiej?",
    "Co bardziej się liczy w społeczeństwie kreatywność, czy praktyczność?",
    "Czy kiedykolwiek posiądziemy wiedzę absolutną?",
    "Czym jest dla ciebie rodzina?",
    "Czy lepiej być osobą wrażliwą i empatyczną, czy jednak odporną na gwałtowne emocje?",
    "Czym kieruje się człowiek w swoim życiu poza egoizmem? Uważasz, że jest coś po za nim?",
    "Czy opłaca się poświęcić swoje ideały i wartości dla krótkotrwałych korzyści?",
    "Czy z czasem tożsamość narodowa społeczeństwa będzie zanikać?",
    "Jeśli wszechświat nie jest nieograniczony, co znajduje się poza jego granicami?",
    "W naturze panuje porządek, czy raczej chaos?",
    "“Co nie jest pożyteczne dla roju, i dla pszczoły nie jest pożyteczne”.",
    "Czy według ciebie oddanie za kraj jest obowiązkiem obywatelskim?",
    "Czy wolny rynek podwyższa poziom naszego życia?",
    "Czy istnieją na świecie kultury lepsze i gorsze?",
    "Czy kolonializm w rzeczywistości rozwinął biedniejsze państwa?",
    "Czy okupacja innego państwa może być moralnie uzasadniona?",
    "Czy każdy naród powinien mieć prawo posiadać własne państwo?",
    "Czy może powstać coś z niczego?",
    "Czy nauki oparte na duchowości zasługują na ich miano?",
    "Czy jeśli wymienimy wszystkie części człowieka na nowe, a więc cały organizm zostanie zastąpiony nowym, to czy pozostaje on tym samym człowiekiem? Od czego to zależy?",
    "Czy da się udowodnić, że ludzie inni niż my sami są samoświadomi?",
    "Jak bardzo rozwiniętą świadomość posiadają zwierzęta? Jak powinniśmy je postrzegać?",
    "Kim jest geniusza? Jak go zdefiniować?",
    "Jak bardzo język, którym mówimy, wpływa na nasz sposób myślenia?",
    "Czy ludzka kreatywność ma granice?",
    "Czy idealny klon nas samych jest nami?",
    "Skąd wiesz, że twoje wspomnienia nie są fałszywe?",
    "Czy śluby homoseksualne powinny być legalne?",
    "Kiedy, i czy w ogóle, odebranie ludzkiego życia jest usprawiedliwione?",
    "Czy zwierzęta posiadają moralność? Z czego ona wynika?",
    "Czy brak religii prowadzi do degeneracji i dekadencji społeczeństwa?",
    "Czy seks pozamałżeński jest niemoralny?",
    "Czy edukacja seksualna w szkołach jest potrzebna?",
    "Jak powinna zmienić się orientacja polityki zagranicznej Polski?",
    "Wysokość trójkąta równobocznego wynosi 3,5 cm. Ile wynosi pole koła opisanego na tym trójkącie?",
    "Czy mieszanie się ras jest dobrym zjawiskiem?",
    "Czy są autorytety, których nie warto kwestionować? Jeśli tak podaj przykład.",
    "Czy człowiek powinien posiadać wrodzone prawa? Czy powinien mieć możliwość zrzeczenia się tych praw?",
    "Czy zwierzęta powinny posiadać więcej praw? Jakie?",
    "Jaka jest różnica między sprawiedliwością, a zemstą?",
    "Czy kradzież jest uzasadniona jeśli jest w stanie uratować życie złodzieja?",
    "Czy prywatność jest prawem człowieka?",
    "Czy przemoc rewolucyjna jest uzasadniona?",
    "Czy propagowanie takich ideologii jak komunizm, nazizm, faszyzm czy inne powinno być karane?",
    "Moralność jest obiektywna czy subiektywna? Dlaczego?",
    "Czy krucjaty przeciwko niewiernym są uzasadnione?",
    "Czy sexwork powinien być zakazany?",
    "Czy istnieje życie po śmierci? Jeśli nie to co się z nami dzieje po?",
    "W jakich sytuacjach wolność słowa powinna być ograniczana?",
    "Czy eutanazja powinna być legalna? Jest to moralne i etyczne?",
    "Czy aborcja powinna być legalna? Jest to moralne i etyczne?",
    "Czy muzyka, która zawiera tematykę szkodliwą społecznie powinna być ocenzurowana?",
    "Czy narkoman powinien być poddany leczeniu czy może izolacji od społeczeństwa?",
    "Czy miłość jest uczuciem, które ogranicza nasze poznanie rzeczywistości, czy raczej je rozszerza?",
    "Na których cechach Jezusa powinniśmy się wzorować?",
    "Jakie poglądy dzielisz z największymi zbrodniarzami?",
    "Czy na religii w szkołach także powinno się omawiać inne religie?",
    "Czy państwo powinno powołać odpowiednia instytucje odpowiedzialna za państwową budowe mieszkań?",
    "Czy zgodziłbyś się na budowę elektrowni atomowej w pobliżu twojego miejsca zamieszkania? Jeśli nie to dlaczego?",
    "Czy kara śmierci jest zawsze zła i niemoralna?",
    "Czy osoby ze skłonnościami pedofilskimi które nie popełniły przestępstw powinny być przymusowo odizolowane od społeczeństwa/wysłane na terapie?",
    "Czy własność jest konieczna do posiadania wolności?",
    "Czy ofiara/rodzina ofiary powinny mieć wpływ na wyrok?",
    "Wysokie podatki są niemoralne.",
    "Ziemia jest zdecydowanie przeludniona.",
    "Świat byłby lepszym miejscem gdyby panowała jedna rasa.",
    "Obozy pracy to dobry sposób karania przestępców.",
    "Obywatele nie mają wpływu na nic, to tylko pozory.",
    "Prawdziwy władza kieruje nami spoza oka opinii publicznej.",
    "Każdy mężczyzna powinien nauczyć się jak bronić siebie i swoją rodzinę przed agresorem.",
    "W przypadku wojny każdy obywatel powinien spełnić swój obowiązek wobec ojczyzny.",
    "Lepiej współpracować z faszystą czy z komunistą?",
    "Byłbym gotów umrzeć za moje wartości (np. w obronie ojczyzny, religii, stylu życia).",
    "Głównym celem małżeństwa jest prokreacja.",
    "Miks OZE + atom to preferowane przeze mnie źródło zasilania.",
    "Przedstawiciele kościoła katolickiego szkodzą mu bardziej od przeciwników KK.",
    "Kościół katolicki powinien być uprzywilejowany ze względu na wielowiekową tradycję i pozytywny wpływ na historię RP.",
    "Głową państwa powinien być duchowny.",
    "Siły generała Franco w hiszpańskiej wojnie domowej to mniejsze zło.",
    "Jeśli państwo nie potrafi zapewnić porządku powinno interweniować wojsko.",
    "Szerzenie i zachęcanie do paranauki powinno być penalizowane.",
    "Świadoma dezinformacja powinna być penalizowana.",
    "Śmierć jednostki to tragedia, miliona to statystyka.",
    "Wojna jest potrzebna dla rozwoju cywilizacji.",
    "Człowiek rodzi się dobrym, dopiero pod wpływem otoczenia/wychowania nabiera cech negatywnych."
];

client.on('ready', function() {
    console.log(client.user.tag);
});


let index = 0;
var interval;

client.on('message', (message) => {
    if (message.content === 'balcerowicz') {
     const response = balcerowicz[Math.floor(Math.random() * balcerowicz.length)];
     message.channel.send(response);
    }
   });

client.on('message', (message) => {
    if (message.content === 'Balcerowicz') {
     const response = balcerowicz[Math.floor(Math.random() * balcerowicz.length)];
     message.channel.send(response);
    }
   });


client.on('message', function(message) {
    if (message.content === "$loop-start") {
            message.channel.send("start") 
         interval = setInterval (function () {
            message.channel.send(seksZPedalami[index])
            .catch(console.error);
			if (index>=seksZPedalami.length-1){index=0}
            else {index++};
        }, 1000*60*60*6); 
    } 
    if (message.content === "$loop-stop") {
        if (interval){
            clearInterval(interval);
            interval=undefined;
            message.channel.send("stop")
        }
        else message.channel.send("brak loopa")
    }
    if (message.content === "$loop-random") {
        message.channel.send("random")
        interval = setInterval (function () {
            message.channel.send("<@&857724440467734548>")
            const random=Math.floor(Math.random()*(seksZPedalami.length-1));
            message.channel.send(seksZPedalami[random])
            .catch(console.error);
        }, 1000*60*60*6); 
    }
});

client.login('ODUzMjg3MzU4NDI5NjU5MTU2.YMTLxw.rIe0zlTPny97VSNJbFmO7n3OB2Q');
