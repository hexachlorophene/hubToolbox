
<html>
<title>HTML Tutorial</title>
<body>

<h1>Hot/Cold Check</h1>
<p>Enter Zip Code</p>


<input type="number" id="zipCode" onkeypress="checkEnter(event)">
<button id="checkButton" onClick="checkInput()">Check</button>
<br>
<H1 id="result"></H1>
<H1 id="upgrade"></H1>
<script>
function checkEnter(ev){
	if(ev.keyCode==13){
		checkInput();
		document.getElementById("zipCode").select();
		}
	}

function checkInput(){
var Hot = false;
var toInt = 0;
var InfoText = "";
toInt = document.getElementById("zipCode").value;
document.getElementById("zipCode").select();

if(toInt<10000 || toInt>99999)
	{
		alert("Invalid Input");
		hot = false;
                infoText = "Invalid Input";
	}

else if ((toInt >= 37300 && toInt <= 37999)
                || (toInt >= 28700 && toInt <= 28999)
                || (toInt >= 30100 && toInt < 30200)
                || (toInt >= 30700 && toInt < 30800)
                || (toInt >= 24200 && toInt < 24400)
//Arkansas
                || (toInt >= 71600 && toInt <= 71999)
                || (toInt >= 72002 && toInt <= 72004)
                || (toInt >= 72006 && toInt <= 72013)
                || (toInt >= 72015 && toInt <= 72020)
                || (toInt >= 72022 && toInt <= 72024)
                || (toInt >= 72026 && toInt <= 72028)
                || (toInt >= 72030 && toInt <= 72035)
                || (toInt >= 72037 && toInt <= 72042)
                || (toInt >= 72045 && toInt <= 72048)
                || (toInt >= 72052 && toInt <= 72061)
                || (toInt >= 72064 && toInt <= 72068)
                || (toInt >= 72070 && toInt <= 72073)
                || (toInt >= 72076 && toInt <= 72079)
                || (toInt >= 72081 && toInt <= 72087)
                || (toInt >= 72089 && toInt <= 72099)
                || (toInt >= 72102 && toInt <= 72107)
                || (toInt == 72111)
                || (toInt >= 72113 && toInt <= 72122)
                || (toInt == 72124)
                || (toInt >= 72126 && toInt <= 72129)
                || (toInt >= 72131 && toInt <= 72152)
                || (toInt >= 72157 && toInt <= 72164)
                || (toInt >= 72166 && toInt <= 72168)
                || (toInt >= 72170 && toInt <= 72199)
                || (toInt >= 72200 && toInt <= 72299)
                || (toInt == 72530)
                || (toInt == 72543)
                || (toInt >= 72545 && toInt <= 72546)
                || (toInt == 72581))
            {
                hot = true;
                infoText = "Hot: Knoxville";
            }
//Whites Creek TN
            else if ((toInt >= 37000 && toInt <= 37299)
                || (toInt >= 38000 && toInt <= 38599)
                || (toInt >= 35000 && toInt <= 35999)
                || (toInt == 36024 || toInt == 36026 || toInt == 36080)
                || (toInt == 36251 || toInt == 36255 || toInt == 36256 || toInt == 36267 || toInt == 36276)
                || (toInt == 36744 || toInt == 36776)
                || (toInt >= 73000 && toInt <= 74999))
            {
                hot = true;
                infoText = "Hot: Whites Creek";
            }
//Charleston WV
            else if ((toInt >= 24700 && toInt <= 25399)
                || (toInt >= 25500 && toInt <= 26699)
                || (toInt >= 26800 && toInt <= 26899))
            {
                hot = true;
                infoText = "Hot: WV";
            }
//Columbus OH
            else if ((toInt >= 43000 && toInt <= 43008) || (toInt >= 43011 && toInt <= 43028)
                || (toInt >= 43030 && toInt <= 43043) || (toInt >= 43045 && toInt <= 43046)
                || (toInt >= 43048 && toInt <= 43059) || (toInt >= 43061 && toInt <= 43069)
                || (toInt == 43071) || (toInt >= 43073 && toInt <= 43077)
                || (toInt >= 43079 && toInt <= 43082) || (toInt == 43085)
                || (toInt >= 43102 && toInt <= 43103) || (toInt == 43105)
                || (toInt >= 43107 && toInt <= 43112) || (toInt >= 43116 && toInt <= 43120)
                || (toInt >= 43122 && toInt <= 43127) || (toInt >= 43129 && toInt <= 43134)
                || (toInt >= 43136 && toInt <= 43139) || (toInt >= 43143 && toInt <= 43144)
                || (toInt >= 43146 && toInt <= 43150) || (toInt == 43155)
                || (toInt >= 43157 && toInt <= 43159) || (toInt >= 43161 && toInt <= 43163)
                || (toInt >= 43165 && toInt <= 43199)
                || (toInt >= 43200 && toInt <= 43299)
                || (toInt >= 43300 && toInt <= 43310) || (toInt >= 43312 && toInt <= 43317)
                || (toInt >= 43320 && toInt <= 43335) || (toInt >= 43337 && toInt <= 43342)
                || (toInt >= 43344 && toInt <= 43356) || (toInt >= 43358 && toInt <= 43359)
                || (toInt >= 43400 && toInt <= 44999) || (toInt >= 45700 && toInt <= 45899)
                || (toInt == 45622) || (toInt == 45651) || (toInt == 45654) || (toInt == 45695) || (toInt == 45698))
            {
                hot = true;
                infoText = "Hot: Columbus";
            }
//Indianapolis IN
            else if ((toInt >= 46000 && toInt <= 47999) || (toInt >= 60900 && toInt <= 60999)
                || (toInt >= 61800 && toInt <= 61999) || (toInt >= 62500 && toInt <= 62599)
                || (toInt >= 62400 && toInt <= 62499
                && toInt != 62411 && toInt != 62412 && toInt != 62418
                && toInt != 62426 && toInt != 62443 && toInt != 62458 && toInt != 62471)
                || (toInt == 62806) || (toInt == 62809) || (toInt == 62811) || (toInt == 62815)
                || (toInt == 62818) || (toInt == 62820) || (toInt == 62823) || (toInt == 62824)
                || (toInt == 62827) || (toInt == 62833) || (toInt == 62837) || (toInt == 62839)
                || (toInt == 62842) || (toInt == 62843) || (toInt == 62844) || (toInt == 62850)
                || (toInt == 62852) || (toInt == 62855) || (toInt == 62858) || (toInt == 62862)
                || (toInt == 62863) || (toInt == 62868) || (toInt == 62878) || (toInt == 62879)
                || (toInt == 62887))
            {
                hot = true;
                infoText = "Hot: Indianapolis";
            }
 //CCHIL IL
            else if ((toInt >= 83200 && toInt <= 83899) || (toInt >= 97000 && toInt <= 97999)
                || (toInt >= 98000 && toInt <= 99499) || (toInt >= 93600 && toInt <= 96199))
            {
                hot = true;
                infoText = "Hot: CCHIL";
            }
//Paducah KY
            else if ((toInt >= 42000 && toInt <= 42099))
            {
                hot = true;
                infoText = "Hot: Paducah";
            }
            else
            {
                hot = false;
                infoText = "Cold (Check for Next Day)";
            }
//updates for and new colds
            if(toInt >=25700  && toInt<=25799 || toInt >= 47100 && toInt <= 47199)
            {
                hot = false;
				infoText = "Cold (Check for Next Day)";
            }
	

if (hot&&(
            (toInt>=37001&&toInt<=37011)|| (toInt >= 37013 && toInt <= 37058)
            || (toInt >= 37060 && toInt <= 37094) || (toInt >= 37096 && toInt <= 37099)
            || (toInt >= 37101 && toInt <= 37109) || (toInt >= 37112 && toInt <= 37165)
            || (toInt >= 37167 && toInt <= 37199)             
            || (toInt >= 37200 && toInt <= 37299)
            || (toInt == 37301) || (toInt == 37305) || (toInt == 37306) || (toInt == 37318) 
            || (toInt == 37319) || (toInt == 37324) || (toInt == 37328) || (toInt == 37330)
            || (toInt == 37334) || (toInt == 37335) || (toInt == 37342) || (toInt == 37301)
            || (toInt >= 37344 && toInt <= 37346) || (toInt == 37348) || (toInt == 37349)
            || (toInt == 37352) || (toInt == 37355) || (toInt >= 37357 && toInt <= 37360)
            || (toInt == 37366) || (toInt == 37382) || (toInt >= 37388 && toInt <= 37390)
            || (toInt >= 37392 && toInt <= 37395) || (toInt >= 37398 && toInt <= 37399)
            || (toInt == 37705) || (toInt == 37707) || (toInt == 37709) || (toInt == 37714)
            || (toInt == 37715) || (toInt == 37721) || (toInt == 37724) || (toInt == 37725)
            || (toInt == 37729) || (toInt == 37730) || (toInt == 37738) || (toInt == 37752)
            || (toInt == 37754) || (toInt == 37757) || (toInt == 37760) || (toInt == 37762)
            || (toInt == 37764) || (toInt == 37766) || (toInt == 37769) || (toInt == 37773)
            || (toInt == 37779)
            || (toInt == 37806) || (toInt == 37807) || (toInt == 37819) || (toInt == 37820) 
            || (toInt == 37824) || (toInt == 37825) || (toInt == 37828)
            || (toInt >= 37847 && toInt <= 37849) || (toInt == 37851) || (toInt >= 37861 && toInt <= 37868)
            || (toInt == 37870) || (toInt == 37871) || (toInt == 37876) || (toInt == 37879)
            || (toInt == 37888)
            || (toInt >= 37900 && toInt <= 37999)
            || (toInt == 38201) || (toInt >= 38221 && toInt <= 38226) || (toInt == 38229) || (toInt == 38231)
            || (toInt >= 38236 && toInt <= 38238) || (toInt == 38241) || (toInt == 38242) || (toInt == 38251)
            || (toInt == 38255) || (toInt == 38256) || (toInt == 38257)
            || (toInt == 38317) || (toInt == 38318) || (toInt == 38320) || (toInt == 38324) 
            || (toInt == 38333) || (toInt == 38341) || (toInt == 38342) || (toInt == 38344) 
            || (toInt == 38387) || (toInt == 38390)
            || (toInt == 38401) || (toInt == 38402) || (toInt == 38451) || (toInt == 38454)
            || (toInt == 38461) || (toInt == 38462) || (toInt == 38474) || (toInt == 38476)
            || (toInt == 38482) || (toInt == 38487) || (toInt == 38488)
            || (toInt >= 38501 && toInt <= 38503) || (toInt == 38505) || (toInt == 38506)
            || (toInt >= 38541 && toInt <= 38545) || (toInt >= 38547 && toInt <= 38549)
            || (toInt == 38551) || (toInt == 38552) || (toInt == 38554) || (toInt == 38560)
            || (toInt == 38562) || (toInt == 38563) || (toInt == 38564)
            || (toInt >= 38567 && toInt <= 38570) || (toInt == 38573) || (toInt == 38575) || (toInt == 38577)
            || (toInt == 38580) || (toInt == 38582) || (toInt == 38588) || (toInt == 38589)
            || (toInt == 43002) || (toInt == 43004) || (toInt == 43007) || (toInt == 43016)
            || (toInt == 43017) || (toInt == 43021) || (toInt == 43026) || (toInt == 43035)
            || (toInt == 43036) || (toInt == 43040) || (toInt == 43041) || (toInt == 43045)
            || (toInt == 43054) || (toInt == 43061) || (toInt == 43064) || (toInt == 43065)
            || (toInt == 43067) || (toInt == 43068) || (toInt == 43069) || (toInt == 43073)
            || (toInt == 43074) || (toInt == 43077) || (toInt == 43081) || (toInt == 43082)
            || (toInt == 43085) || (toInt == 43086)
            || (toInt == 43103) || (toInt == 43109) || (toInt == 43110) || (toInt == 43116)
            || (toInt == 43117) || (toInt == 43119) || (toInt == 43123) || (toInt == 43125)
            || (toInt == 43126) || (toInt == 43136) || (toInt == 43137) || (toInt == 43143)
            || (toInt == 43146) || (toInt == 43147) || (toInt == 43162) || (toInt == 43194)
            || (toInt == 43195) || (toInt == 43199)
            || (toInt >= 43200 && toInt <= 43299)
            || (toInt == 43310) || (toInt == 43316) || (toInt == 43324) || (toInt == 43331)
            || (toInt == 43333) || (toInt == 43346) || (toInt == 43347) || (toInt == 43348)
            || (toInt == 43413) || (toInt == 43437) || (toInt == 43457) || (toInt == 43466)
            || (toInt == 43467)
            || (toInt == 43516) || (toInt == 43529)
            || (toInt == 44802) || (toInt == 44804) || (toInt == 44817) || (toInt == 44830)
            || (toInt == 44844) || (toInt == 44853)
            || (toInt == 45801) || (toInt == 45802) || (toInt >= 45804 && toInt <= 45810)
            || (toInt == 45812) || (toInt >= 45814 && toInt <= 45817) || (toInt == 45819) || (toInt == 45820)
            || (toInt == 45822) || (toInt >= 45826 && toInt <= 45828) || (toInt == 45830) || (toInt == 45832)
            || (toInt == 45833) || (toInt == 45835) || (toInt == 45836) || (toInt >= 45838 && toInt <= 45841)
            || (toInt >= 45843 && toInt <= 45846) || (toInt >= 45848 && toInt <= 45851) || (toInt == 45853)
            || (toInt == 45854) || (toInt == 45856) || (toInt >= 45858 && toInt <= 45860)
            || (toInt >= 45862 && toInt <= 45873)
            || (toInt >= 46000 && toInt <= 46299)
            || (toInt == 46702) || (toInt == 46704) || (toInt == 46711) || (toInt == 46713) 
            || (toInt == 46714) || (toInt == 46723) || (toInt == 46725) || (toInt == 46731) 
            || (toInt == 46733) || (toInt == 46740) || (toInt == 46741) || (toInt == 46743)
            || (toInt == 46745) || (toInt == 46748) || (toInt == 46750) || (toInt == 46759)
            || (toInt == 46764) || (toInt == 46765) || (toInt == 46766) || (toInt == 46769)
            || (toInt == 46770) || (toInt == 46772) || (toInt == 46773) || (toInt == 46774)
            || (toInt == 46777) || (toInt == 46778) || (toInt == 46780) || (toInt == 46781)
            || (toInt == 46782) || (toInt == 46783) || (toInt == 46787) || (toInt == 46791)
            || (toInt == 46792) || (toInt == 46797)
            || (toInt >= 46800 && toInt <= 46899)
            || (toInt >= 46900 && toInt <= 46909) || (toInt == 46911) || (toInt >= 46913 && toInt <= 46920)
            || (toInt >= 46923 && toInt <= 46927) || (toInt >= 46929 && toInt <= 46932) || (toInt == 46936)
            || (toInt == 46937) || (toInt == 46942) || (toInt >= 46947 && toInt <= 46950) || (toInt == 46958)
            || (toInt == 46959) || (toInt == 46961) || (toInt == 46965) || (toInt == 46966) || (toInt == 46967)
            || (toInt >= 46970 && toInt <= 46973) || (toInt == 46977) || (toInt == 46978) || (toInt == 46979)
            || (toInt == 46988) || (toInt == 46994) || (toInt == 46995) || (toInt == 46998) || (toInt == 46999)
            || (toInt >= 47000 && toInt <= 47499)
            || (toInt >= 47501 && toInt <= 47512) || (toInt >= 47516 && toInt <= 47519)
            || (toInt == 47522) || (toInt == 47524) || (toInt == 47526) || (toInt == 47528) 
            || (toInt == 47529) || (toInt == 47530) || (toInt == 47533) || (toInt == 47534)
            || (toInt == 47535) || (toInt == 47538) || (toInt == 47539) || (toInt == 47540)
            || (toInt == 47543) || (toInt == 47544) || (toInt == 47548) || (toInt == 47553)
            || (toInt == 47554) || (toInt == 47555) || (toInt >= 47557 && toInt <= 47563)
            || (toInt >= 47565 && toInt <= 47573) || (toInt == 47578) || (toInt == 47581)
            || (toInt == 47582) || (toInt == 47583) || (toInt == 47587) || (toInt == 47589)
            || (toInt >= 47591&& toInt <= 47597)
            || (toInt >= 47600 && toInt <= 47999)
            || (toInt == 60918) || (toInt == 60924) || (toInt == 60926) || (toInt == 60932)
            || (toInt == 60933) || (toInt == 60936) || (toInt == 60939) || (toInt == 60942)
            || (toInt == 60948) || (toInt == 60949) || (toInt == 60952) || (toInt == 60953)
            || (toInt == 60957) || (toInt == 60960) || (toInt == 60962) || (toInt == 60963)
            || (toInt == 60967) || (toInt == 60973)
            || (toInt == 61801) || (toInt == 61802) || (toInt == 61803)
            || (toInt >= 61810 && toInt <= 61818) || (toInt >= 61820 && toInt <= 61822)
            || (toInt >= 61824 && toInt <= 61826) || (toInt >= 61830 && toInt <= 61834)
            || (toInt >= 61839 && toInt <= 61859) || (toInt >= 61862 && toInt <= 61866)
            || (toInt >= 61870 && toInt <= 61878) || (toInt == 61880) || (toInt == 61882)
            || (toInt == 61883) || (toInt == 61884)
            || (toInt == 61919) || (toInt == 61924) || (toInt == 61932) || (toInt == 61940) 
            || (toInt == 61941) || (toInt == 61942) || (toInt == 61953) || (toInt == 61956)
            || (toInt == 62410) || (toInt == 62411) || (toInt == 62413) || (toInt == 62417)
            || (toInt == 62418) || (toInt == 62419) || (toInt == 62421) || (toInt == 62425)
            || (toInt == 62426) || (toInt == 62427) || (toInt == 62432) || (toInt == 62433)
            || (toInt == 62434) || (toInt == 62439) || (toInt == 62443) || (toInt == 62446)
            || (toInt == 62448) || (toInt == 62449) || (toInt == 62450) || (toInt == 62451)
            || (toInt == 62452) || (toInt == 62454) || (toInt == 62458) || (toInt == 62459)
            || (toInt == 62460) || (toInt == 62464) || (toInt == 62466) || (toInt == 62471)
            || (toInt == 62475) || (toInt == 62476) || (toInt == 62477) || (toInt == 62478)
            || (toInt == 62480) || (toInt == 62481)
            || (toInt >= 62800 && toInt <= 62899)
              )
            )
        {
            document.getElementById("upgrade").innerHTML = "Upgrade: Yes";
        }
        else
        {
            document.getElementById("upgrade").innerHTML = "Upgrade: No";
        }
if(hot){
document.getElementById("result").sytle.color="red";
}else{
document.getElementById("result").style.color="blue";
}

document.getElementById("result").innerHTML = toInt + ": " + infoText;
}
</script>
</body>
</html>
