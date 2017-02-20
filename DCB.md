
#Mostkowanie centrum danych DCB

###Opis funkcji

Funckja mostkowania centrum danych (DCB)to zestaw standardów IEEE (Institute of Electrical and Electronics Engineers umożliwiających działanie konwergentnych sieci szkieletowych w centrach danych, w których magazyn, sieć danych, komunikacja IPC klastrów i ruch związany z zarządzaniem działają w tej samej infrastrukturze sieci Ethernet.
Funkcja DCB zapewnia sprzętowe możliwości przydziału przepustowości dla określonego typu ruchu i zwiększa niezawodnośc transportu w sieci Ethernet dzięki sterowaniu przepływem na podstawie priorytetu. Przydzielanie przepustowości oparte na sprzęcie jest niezbędne, gdy ruch omija system operacyjny i jest odciążany do karty sieci konwergentnej, która może obsługiwać interfejs iSCSI, zdalny bezpośredni dostęp do Pamięci (RDMA) przez konwergentną sieć Ethernet lub protokół FCoE (Fibre Channel over Ethernet). Sterowanie przepływem oparte na priorytetach jest niezbędne, jeśli protokół warstwy wyższej, np. Fiber Channel, zakłada bezstratny transport w warstwie niższej.

###Zastosowanie praktyczne

W wielu przedsiębiorstwach istnieją duże instalacje sieci magazynowania (SAN) Fiber Channel (FC) dla usługi magazynowania. Sieć SAN FC wymaga zastosowania specjalnych kart sieciowych na serwerach i przełącznikach FC w sieci. Ogólnie wdrażanie sprzętu sieci FC jest znacznie droższe niż wdrażanie sprzętu sieci Ethernet, co powoduje duże wydatki inwestycyjne. Ponadto posiadanie oddzielnego adaptera i przełącznika do obsługi ruchu sieciowego Ethernet i SAN FC wymaga dodatkowej przestrzeni, mocy i wydajności chłodzenia w centrum danych. O wiele korzystniejsze jest scalanie technologii FC z rozwiązaniami sprzętowymi sieci Ethernet.

Dla firm któr już posiadają duże sieci FC SAN, funkcja DCB umożliwia utworzenie konwergentnej sieci szkieletowej.Taka konwergentna sieć szkieletowa utworzona przy użyciu funkcji DCB może zmniejszyć przyszły całkowity koszt posiadania i ułatwić zarządzanie. W sytuacjik iedy dostawca usług hostingowych wdrożył lub zamierza wdrożyć rozwiązanie magazynowania iSCSI, funkcja DCB może zapewnić sprzętową rezerwację przepustowości dla ruchu iSCSI w celu zapewnienia izolacji wydajności.

###DCB a oprogramowanie Windows Server 2012

Zastosowanie funkcji DCB w systemie Windows Server® 2012 eliminuje wiele problemów, które wystepują w sytuacji kiedy rozwiązania konwergentnej sieci szkieletowej pochodzą od wielu producentów OEM. Implementacja rozwiązań własnościowych dostarczonych przez producentów sprawia , że mogą one nie współpracować ze sobą, wykazywać trudności w zarządzaniu i mające różne harmonogramy konserwacji oprogramowania. W przeciwieństwie do do tych rozwiązań funkcja DCB w systemie Windows Server® 2012 jest oparta na standardach i dosyć łatwa do wdrożenia i zarządzania. 

###Ważne funcke reaizowane poprzez DCB

1. Zapewnia współpracę między kartami sieciowymi i przełącznikami z obsługą funkcji DCB.
2. Zapewnia bezstratną transmisję za pośrednictwem sieci Ethernet między komputerem z systemem Windows Server® 2012 i sąsiadującym przełącznikiem przez włączenie w karcie sieciowej sterowania przepływem na podstawie priorytetów.
3. Umożliwia przydzielenie wartości procentowej przepustowości do kontroli ruchu, gdzie kontrola ruchu może składać się z co najmniej jednej klasy ruchu rozróżnianej na podstawie wartości 802.1p.
4. Umożliwia administratorom serwera lub administratorom sieci przypisanie aplikacji do określonej klasy ruchu lub priorytetu na podstawie dobrze znanych protokołów, dobrze znanego portu TCP/UDP lub portu NetworkDirect używanego przez tę aplikację.
5. Zapewnia możliwość zarządzania funkcją DCB przy użyciu infrastruktury Instrumentacji zarządzania Windows (WMI) i programu Windows PowerShell w systemie Windows Server® 2012.
6. Zapewnia możliwość zarządzania funkcją DCB przy użyciu zasad grupy w systemie Windows Server® 2012.
7. Obsługuje współistnienie rozwiązań jakości usług (QoS) w systemie Windows Server® 2012.
