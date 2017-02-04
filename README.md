# AKGRadioButton
`AKGRadioButton ` is an easy to use and highly customizable radio buttons control for iOS. It's a subclass of `UIButton`, and works smoothly with`Swift`.


Make Object of AKGRadioButtonModel like :
 eg   :
 
        let maleButton = AKGRadioButtonModel(lblText : "Male" ,identifire : "Male" ,selected : true)
        let femaleButton = AKGRadioButtonModel(lblText : "Female" ,identifire : "Female" ,selected : false)
        let gayButton = AKGRadioButtonModel(lblText : "Other" ,identifire : "Other" ,selected : false)
      
        akgRadioButtonModel = [maleButton,femaleButton,gayButton]

 
Initialised AKGRadioButtonGroupView object and pass parameter Group name ,AKGRadioButtonModel array, and positions
 eg    : 
 
        let  akgRBGroupView = AKGRadioButtonGroupView(akgRadioButtonModel : akgRadioButtonModel! ,akgRadioButtonGroupName : "Gender" , akgRadioButtonGroupPosstion : size)
        akgRBGroupView.setupView()
        akgRBGroupView.delegate = self
        self.view.addSubview(akgRBGroupView)

After selection Radio Button result will got in delegate
eg    :
   
     func selectedResult(resultObject:AKGRadioButtonModel){
        print("Selected Radio Button -> \(resultObject.lblText)")
     }



