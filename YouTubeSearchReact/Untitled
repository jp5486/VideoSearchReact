import React, { Component } from 'react';

// const SearchBar = () => {
//   return <input />;
// };

// refector 1, with component from import
// class SearchBar extends Component {
//   render() {
//     return <input onChange={this.handleInputChange} />
//   }

//   handleInputChange(event) {
//     console.log(event.target.value)
//   }
// }


//refactor out handleInputChange
class SearchBar extends Component {
  constructor(props) {
    super(props);

    this.state = { keyword: '' };
  }

  render() {
    return (
      <div className="search-bar">
        <input
          value={this.state.keyword}
          onChange={event => this.handleInputChange(event.target.value) } />
      </div>
    );
  }
  // onChange={event => this.setState({ term: event.target.value})} />

  handleInputChange(term){
    this.setState({keyword: term});
    this.props.handleSearchTermChange(term);
  }
}


export default SearchBar;
