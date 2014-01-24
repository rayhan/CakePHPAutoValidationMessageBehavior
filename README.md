**Put ValidationMessageBehavior.php inside app/Model/Behavior folder**


**Attach behavior in your CakePHP Model**

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

Supports CakePHP 2.xxx versions.
