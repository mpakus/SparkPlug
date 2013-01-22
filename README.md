A scaffolding library inspired by Ruby on Rails scaffolding. Adds the ability to generate basic CRUD functionality for any given database table.

Original code - http://code.google.com/p/sparkplug/ works with lower than 2 version of CodeIgniter, I'm just fixed scaffolding method for CI ver 2.x and it's works.

author Pascal Kriete
small fixes for CI ver.2.x by MpaK

<code>
<?php

class Partners extends CI_Controller {

    public function __construct() {
		parent::__construct();
    }

    public function index() {
		$this->load->library( 'sparkPlug' );
		$this->sparkplug->set_table( 'partners' );
		$this->sparkplug->scaffold();
    }
}

</code>