# EC2 Image Builder STIG components<a name="image-builder-stig"></a>

Security Technical Implementation Guides \(STIGs\) are the configuration standards created by the Defense Information Systems Agency \(DISA\) to secure information systems and software\. To make your systems compliant with STIG standards, you must install, configure, and test a variety of security settings\. 

EC2 Image Builder provides STIG components to help you quickly build compliant images for STIG standards\. These STIG components scan for misconfigurations and run a remediation script\. There are no additional charges for using STIG\-compliant components\. 

**Compliance levels**
+ **High \(Category I\) **

  The most severe risk\. It includes any vulnerability that can result in loss of confidentiality, availability, or integrity\.
+ **Medium \(Category II\) **

  Any vulnerability that could result in loss of confidentiality, availability, or integrity\. These risks could be mitigated\.
+ **Low \(Category III\) **

  Any vulnerability that degrades measures to protect against loss of confidentiality, availability, or integrity\.

**Topics**
+ [Windows STIG components](#base-os-stig)
+ [Linux STIG components](#ie-os-stig)

## Windows STIG components<a name="base-os-stig"></a>

Windows STIG components are designed for standalone servers and apply Local Group Policy\. STIG\-compliant components install InstallRoot on Windows AMIs from the Department of Defense \(DoD\) to install and update the DoD certificates\. They also remove unnecessary certificates to maintain STIG compliance\. 

### STIG\-Build\-Windows\-Low version 1\.2\.0<a name="ib-windows-stig-low"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.
+ **Windows Server 2019 STIG V1 Release 5:**

  V\-93233, V\-93235, V\-93237, V\-93259, V\-93261, V\-93309, V\-93409, and V\-93541
+ **Windows Server 2016 STIG V1 Release 12:**

  V\-73499, V\-73501, V\-73503, V\-73505, V\-73543, V\-73563, and V\-73705
+ **Windows Server 2012 R2 STIG V2 Release 19:**

  V\-1075, V\-1128, V\-1136, V\-1151, V\-1165, V\-1172, V\-1173, V\-1174, V\-3373, V\-4108, V\-4110, V\-4111, V\-4112, V\-4113, V\-4116, V\-4438, V\-4442, V\-4445, V\-11806, V\-14232, V\-15672, V\-15686, V\-15687, V\-15701, V\-15702, V\-15703, V\-15704, V\-15707, V\-15718, V\-21955, V\-21956, V\-21960, V\-21961, V\-21963, V\-21964, V\-21965, V\-21967, V\-21969, V\-21970, V\-21971, V\-28504, V\-36673, V\-36677, V\-36678, V\-36696, V\-36697, V\-36776, V\-36777, and V\-43241
+ **Microsoft \.NET Framework 4\.0 STIG V1 Release 9:**

  No STIG settings are applied to the Microsoft \.NET Framework for Category III vulnerabilities\.
+ **Windows Firewall STIG V1 Release 7:**

  V\-17425, V\-17426, V\-17427, V\-17435, V\-17436, V\-17437, V\-17445, V\-17446, and V\-17447
+ **Internet Explorer 11 STIG V1 Release 19:**

  V\-46477, V\-46629, and V\-97527

### STIG\-Build\-Windows\-Medium version 1\.2\.0<a name="ib-windows-stig-medium"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.

**Note**  
The STIG\-Build\-Windows\-Medium components include all STIG settings that Image Builder applies to STIG\-Build\-Windows\-Low components, in addition to the STIG settings that are applied specifically for Category II vulnerabilities\.
+ **Windows Server 2019 STIG V1 Release 5:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for this operating system, plus V\-92965, V\-92967, V\-92969, V\-92971, V\-92973, V\-92979, V\-92981, V\-92983, V\-92987, V\-92989, V\-93007, V\-93009, V\-93011, V\-93015, V\-93017, V\-93045, V\-93053, V\-93055, V\-93059, V\-93063, V\-93067, V\-93069, V\-93071, V\-93073, V\-93075, V\-93079, V\-93081, V\-93083, V\-93085, V\-93087, V\-93089, V\-93091, V\-93093, V\-93095, V\-93097, V\-93099, V\-93101, V\-93103, V\-93105, V\-93107, V\-93109, V\-93111, V\-93113, V\-93115, V\-93117, V\-93119, V\-93141, V\-93143, V\-93145, V\-93151, V\-93153, V\-93155, V\-93157, V\-93159, V\-93161, V\-93163, V\-93165, V\-93167, V\-93169, V\-93171, V\-93173, V\-93175, V\-93177, V\-93179, V\-93181, V\-93197, V\-93199, V\-93239, V\-93243, V\-93249, V\-93251, V\-93253, V\-93255, V\-93257, V\-93263, V\-93265, V\-93267, V\-93269, V\-93285, V\-93287, V\-93293, V\-93295, V\-93297, V\-93299, V\-93303, V\-93305, V\-93307, V\-93311, V\-93313, V\-93315, V\-93317, V\-93319, V\-93335, V\-93339, V\-93367, V\-93383, V\-93385, V\-93387, V\-93389, V\-93391, V\-93393, V\-93395, V\-93397, V\-93399, V\-93401, V\-93403, V\-93405, V\-93407, V\-93411, V\-93413, V\-93415, V\-93421, V\-93423, V\-93425, V\-93427, V\-93429, V\-93431, V\-93433, V\-93435, V\-93445, V\-93453, V\-93455, V\-93459, V\-93463, V\-93469, V\-93471, V\-93477, V\-93479, V\-93487, V\-93489, V\-93491, V\-93493, V\-93495, V\-93497, V\-93499, V\-93501, V\-93505, V\-93517, V\-93521, V\-93523, V\-93525, V\-93527, V\-93529, V\-93533, V\-93547, V\-93549, V\-93551, V\-93553, V\-93555, V\-93557, V\-93559, V\-93561, V\-93563, V\-93565, and V\-102625
+ **Windows Server 2016 STIG V1 Release 12:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for this operating system, plus V\-73287, V\-73291, V\-73293, V\-73295, V\-73297, V\-73299, V\-73301, V\-73309, V\-73311, V\-73313, V\-73315, V\-73317, V\-73319, V\-73321, V\-73323, V\-73413, V\-73415, V\-73419, V\-73423, V\-73427, V\-73429, V\-73431, V\-73433, V\-73443, V\-73445, V\-73447, V\-73449, V\-73451, V\-73453, V\-73455, V\-73457, V\-73459, V\-73461, V\-73463, V\-73465, V\-73467, V\-73469, V\-73471, V\-73473, V\-73475, V\-73477, V\-73479, V\-73481, V\-73483, V\-73487, V\-73489, V\-73491, V\-73493, V\-73497, V\-73507, V\-73511, V\-73521, V\-73525, V\-73527, V\-73529, V\-73531, V\-73537, V\-73539, V\-73541, V\-73551, V\-73553, V\-73555, V\-73557, V\-73559, V\-73561, V\-73565, V\-73567, V\-73569, V\-73571, V\-73573, V\-73575, V\-73577, V\-73579, V\-73581, V\-73583, V\-73587, V\-73589, V\-73591, V\-73595, V\-73597, V\-73601, V\-73603, V\-73605, V\-73607, V\-73609, V\-73627, V\-73633, V\-73635, V\-73637, V\-73639, V\-73641, V\-73643, V\-73645, V\-73653, V\-73655, V\-73657, V\-73661, V\-73663, V\-73673, V\-73677, V\-73679, V\-73681, V\-73683, V\-73685, V\-73693, V\-73695, V\-73697, V\-73699, V\-73707, V\-73709, V\-73711, V\-73713, V\-73715, V\-73717, V\-73719, V\-73721, V\-73727, V\-73733, V\-73739, V\-73743, V\-73745, V\-73749, V\-73753, V\-73759, V\-73763, V\-73767, V\-73771, V\-73775, V\-73781, V\-73783, V\-73785, V\-73787, V\-73789, V\-73793, V\-73795, V\-73797, V\-73799, V\-73801, V\-73803, V\-73807, V\-73809, V\-78123, V\-78125, V\-90359, V\-90361, and V\-102623
+ **Windows Server 2012 R2 STIG V2 Release 19:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for this operating system, plus V\-1070, V\-1097, V\-1098, V\-1099, V\-1104, V\-1105, V\-1107, V\-1113, V\-1141, V\-1150, V\-1154, V\-1155, V\-1157, V\-1162, V\-1163, V\-1164, V\-1166, V\-1171, V\-3374, V\-3377, V\-3378, V\-3380, V\-3381, V\-3382, V\-3385, V\-3449, V\-3453, V\-3454, V\-3455, V\-3456, V\-3469, V\-3470, V\-3479, V\-3480, V\-3481, V\-3666, V\-4447, V\-4448, V\-6831, V\-6832, V\-6833, V\-6836, V\-14228, V\-14229, V\-14230, V\-14234, V\-14235, V\-14236, V\-14237, V\-14239, V\-14240, V\-14241, V\-14242, V\-14243, V\-14247, V\-14249, V\-14253, V\-14259, V\-14260, V\-14261, V\-14268, V\-14269, V\-14270, V\-15666, V\-15667, V\-15674, V\-15682, V\-15683, V\-15684, V\-15685, V\-15696, V\-15697, V\-15698, V\-15699, V\-15700, V\-15705, V\-15706, V\-15722, V\-15727, V\-15991, V\-15997, V\-15998, V\-15999, V\-16000, V\-16008, V\-16020, V\-16021, V\-16048, V\-21950, V\-21951, V\-21952, V\-21953, V\-21954, V\-21980, V\-26469, V\-26470, V\-26472, V\-26473, V\-26474, V\-26478, V\-26480, V\-26481, V\-26482, V\-26483, V\-26484, V\-26485, V\-26486, V\-26487, V\-26488, V\-26489, V\-26490, V\-26492, V\-26493, V\-26494, V\-26496, V\-26498, V\-26499, V\-26500, V\-26504, V\-26506, V\-26529, V\-26530, V\-26533, V\-26535, V\-26537, V\-26538, V\-26539, V\-26540, V\-26541, V\-26542, V\-26543, V\-26546, V\-26547, V\-26548, V\-26549, V\-26550, V\-26551, V\-26552, V\-26553, V\-26555, V\-26557, V\-26558, V\-26575, V\-26576, V\-26577, V\-26578, V\-26579, V\-26580, V\-26581, V\-26582, V\-26600, V\-26604, V\-26605, V\-26606, V\-32272, V\-32274, V\-36656, V\-36657, V\-36667, V\-36668, V\-36679, V\-36680, V\-36681, V\-36684, V\-36687, V\-36698, V\-36700, V\-36707, V\-36708, V\-36709, V\-36713, V\-36714, V\-36719, V\-36720, V\-36773, V\-40200, V\-40202, V\-40204, V\-40206, V\-40237, V\-43238, V\-43239, V\-43240, V\-43245, V\-57633, V\-57639, V\-72753, V\-73519, V\-73523, V\-73805, V\-78057, V\-78059, V\-78061, V\-78063, V\-80473, V\-80475, V\-80477, and V\-102619
+ **Microsoft \.NET Framework 4\.0 STIG V1 Release 9:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for the Microsoft \.NET Framework, plus V\-81495
+ **Windows Firewall STIG V1 Release 7:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for Windows Firewall, plus V\-17415, V\-17416, V\-17417, V\-17419, V\-17429, and V\-17439
+ **Internet Explorer 11 STIG V1 Release 19:**

  Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for Internet Explorer 11, plus V\-46473, V\-46475, V\-46481, V\-46483, V\-46501, V\-46507, V\-46509, V\-46511, V\-46513, V\-46515, V\-46517, V\-46521, V\-46523, V\-46525, V\-46543, V\-46545, V\-46547, V\-46549, V\-46553, V\-46555, V\-46573, V\-46575, V\-46577, V\-46579, V\-46581, V\-46583, V\-46587, V\-46589, V\-46591, V\-46593, V\-46597, V\-46599, V\-46601, V\-46603, V\-46605, V\-46607, V\-46609, V\-46615, V\-46617, V\-46619, V\-46621, V\-46625, V\-46633, V\-46635, V\-46637, V\-46639, V\-46641, V\-46643, V\-46645, V\-46647, V\-46649, V\-46653, V\-46663, V\-46665, V\-46669, V\-46681, V\-46685, V\-46689, V\-46691, V\-46693, V\-46695, V\-46701, V\-46705, V\-46709, V\-46711, V\-46713, V\-46715, V\-46717, V\-46719, V\-46721, V\-46723, V\-46725, V\-46727, V\-46729, V\-46731, V\-46733, V\-46779, V\-46781, V\-46787, V\-46789, V\-46791, V\-46797, V\-46799, V\-46801, V\-46807, V\-46811, V\-46815, V\-46819, V\-46829, V\-46841, V\-46847, V\-46849, V\-46853, V\-46857, V\-46859, V\-46861, V\-46865, V\-46869, V\-46879, V\-46883, V\-46885, V\-46889, V\-46893, V\-46895, V\-46897, V\-46903, V\-46907, V\-46921, V\-46927, V\-46939, V\-46975, V\-46981, V\-46987, V\-46995, V\-46997, V\-46999, V\-47003, V\-47005, V\-47009, V\-64711, V\-64713, V\-64715, V\-64717, V\-64719, V\-64721, V\-64723, V\-64725, V\-64729, V\-72757, V\-72759, V\-72761, V\-72763, V\-75169, and V\-75171

### STIG\-Build\-Windows\-High version 1\.2\.0<a name="ib-windows-stig-high"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=windows)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.

**Note**  
The STIG\-Build\-Windows\-High components include all STIG settings that Image Builder applies to STIG\-Build\-Windows\-Low and STIG\-Build\-Windows\-Medium components, in addition to the STIG settings that are applied specifically for Category I vulnerabilities\.
+ **Windows Server 2019 STIG V1 Release 5:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for this operating system, plus V\-93065, V\-93201, V\-93215, V\-93279, V\-93289, V\-93291, V\-93301, V\-93373, V\-93375, V\-93377, V\-93465, V\-93467, V\-93503, V\-93507, V\-93537, and V\-93539
+ **Windows Server 2016 STIG V1 Release 12:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for this operating system, plus V\-73325, V\-73545, V\-73547, V\-73549, V\-73585, V\-73593, V\-73599, V\-73621, V\-73665, V\-73667, V\-73669, V\-73675, V\-73687, V\-73691, and V\-73755
+ **Windows Server 2012R2 STIG V2 Release 19:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for this operating system, plus V\-1093, V\-1102, V\-1153, V\-2372, V\-2374, V\-3337, V\-3339, V\-3343, V\-3344, V\-3379, V\-4443, V\-6834, V\-18010, V\-21973, V\-22692, V\-26070, V\-26283, V\-26479, V\-34974, V\-36712, and V\-36718
+ **Microsoft \.NET Framework 4\.0 STIG V1 Release 9:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for the Microsoft \.NET Framework\. No additional STIG settings are applied for Category I vulnerabilities\.
+ **Windows Firewall STIG V1 Release 7:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for Windows Firewall, plus V\-17418, V\-17428, and V\-17438
+ **Internet Explorer 11 STIG V1 Release 19:**

  Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for Internet Explorer 11\. No additional STIG settings are applied for Category I vulnerabilities\.

## Linux STIG components<a name="ie-os-stig"></a>

The following sections contain information about Linux STIG components\. Currently, these components are supported only on Amazon Linux 2 configurations, which use the Red Hat Enterprise Linux \(RHEL\) 7 STIG settings\.

### STIG\-Build\-Linux\-Low version 2\.8\.0<a name="ib-linux-stig-low"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=operating-systems%2Cunix-linux)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.

**RHEL 7 STIG V2 Release 8:**

V\-71987, V\-72003, and V\-72059

### STIG\-Build\-Linux\-Medium version 2\.8\.0<a name="ib-linux-stig-medium"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=operating-systems%2Cunix-linux)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.

**Note**  
The STIG\-Build\-Linux\-Medium components include all STIG settings that Image Builder applies to STIG\-Build\-Linux\-Low components, in addition to the STIG settings that are applied specifically for Category II vulnerabilities\.

**RHEL 7 STIG V2 Release 8:**

Includes all STIG settings that Image Builder applies for Category III \(Low\) vulnerabilities for this operating system, plus V\-71905, V\-71907, V\-71909, V\-71911, V\-71913, V\-71915, V\-71917, V\-71919, V\-71921, V\-71923, V\-71925, V\-71933, V\-71935, V\-71941, V\-71943, V\-71945, V\-71951, V\-71959, V\-71983, V\-71985, V\-71995, V\-72013, V\-72095, V\-72097, V\-72099, V\-72101, V\-72103, V\-72105, V\-72107, V\-72109, V\-72111, V\-72113, V\-72115, V\-72117, V\-72119, V\-72121, V\-72123, V\-72125, V\-72127, V\-72129, V\-72131, V\-72133, V\-72135, V\-72137, V\-72139, V\-72141, V\-72145, V\-72147, V\-72149, V\-72151, V\-72153, V\-72155, V\-72157, V\-72159, V\-72161, V\-72163, V\-72165, V\-72167, V\-72171, V\-72173, V\-72175, V\-72177, V\-72179, V\-72183, V\-72185, V\-72187, V\-72189, V\-72191, V\-72197, V\-72199, V\-72201, V\-72203, V\-72205, V\-72207, V\-72221, V\-72223, V\-72233, V\-72235, V\-72237, V\-72241, V\-72243, V\-72245, V\-72247, V\-72249, V\-72253, V\-72259, V\-72261, V\-72263, V\-72265, V\-72267, V\-72283, V\-72285, V\-72287, V\-72289, V\-72291, V\-72293, V\-72297, V\-72307, V\-72309, V\-72319, V\-72417, V\-72433, V\-73159, V\-73165, V\-73167, V\-73171, V\-73173, V\-73175, V\-77821, V\-77825, V\-78999, V\-79001, V\-81003, V\-92251, and V\-92253

### STIG\-Build\-Linux\-High version 2\.8\.0<a name="ib-linux-stig-high"></a>

The following list contains STIG settings that are applied to your image\. Some STIG settings are not automatically applied due to organization\-specific policies, technical limitations, or both\. For a complete list, see the [STIGs Document Library](https://public.cyber.mil/stigs/downloads/?_dl_facet_stigs=operating-systems%2Cunix-linux)\. For information about how to view the complete list, see [How to View SRGs and STIGs ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/doc/HOW_TO_VIEW_SRGs_and_STIGs.doc)\.

**Note**  
The STIG\-Build\-Linux\-High components include all STIG settings that Image Builder applies to STIG\-Build\-Linux\-Low and STIG\-Build\-Linux\-Medium components, in addition to the STIG settings that are applied specifically for Category I vulnerabilities\.

**RHEL 7 STIG V2 Release 8:**

Includes all STIG settings that Image Builder applies for Categories II and III \(Medium and Low\) vulnerabilities for this operating system, plus V\-71939, V\-71967, V\-71969, V\-71977, V\-71979, V\-71993, V\-72077, V\-72079, V\-72299, V\-72301, and V\-72303