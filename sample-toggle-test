define([
  'chai',
  'simulant',
  'rvc!components/inputs/toggle'
], function(
  chai,
  simulant,
  Component
){

  var expect = chai.expect;

  describe('Toggle Component', function() {

    before(function() {
      this.container = document.createElement('div');
      document.body.appendChild(this.container);
    });

    it('click should work', function() {

      var component = new Component({
        el: this.container
      });

      expect(component.data.value).to.equal(false);
      simulant.fire(component.find('.toggle'), 'click', { button: 1, which: 2 });
      expect(component.data.value).to.equal(true);
    });

  });

});

