**Attach behavior in your model**

	public $actsAs = array('ValidationMessage');

**Define Validation Rule**

	public $validate = array(
		'slug' => array(
			'notempty',
			'isUnique'
		),
		'content' => array(
			'alphanumer',
		),
	);

A validation message will automatically be attached to the rule, you don't have to explicitly specify the message;
